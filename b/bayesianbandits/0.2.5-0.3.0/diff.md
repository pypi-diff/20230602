# Comparing `tmp/bayesianbandits-0.2.5.tar.gz` & `tmp/bayesianbandits-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.2.5.tar", max compression
+gzip compressed data, was "bayesianbandits-0.3.0.tar", max compression
```

## Comparing `bayesianbandits-0.2.5.tar` & `bayesianbandits-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/LICENSE
--rw-r--r--   0        0        0     1191 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/README.md
--rw-r--r--   0        0        0     2740 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3991 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    16613 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    27961 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5108 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2445 2023-03-10 17:35:49.517791 bayesianbandits-0.2.5/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-03-10 17:35:49.521790 bayesianbandits-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 bayesianbandits-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/README.md
+-rw-r--r--   0        0        0     2740 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3681 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    18168 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    28409 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5122 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2655 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      705 2023-06-02 18:56:02.805498 bayesianbandits-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.3.0/PKG-INFO
```

### Comparing `bayesianbandits-0.2.5/LICENSE` & `bayesianbandits-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.2.5/README.md` & `bayesianbandits-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -8,28 +8,20 @@
 import numpy as np
 
 from bayesianbandits import Bandit, Arm, epsilon_greedy, DirichletClassifier
 
 def reward_func(x):
     return np.take(x, 0, axis=-1)
 
-def action1_func():
-    # do action 1
-    ...
-
-def action2_func():
-    # do action 2
-    ...
-
 clf = DirichletClassifier({"yes": 1.0, "no": 1.0})
 policy = epsilon_greedy(0.1)
 
 class Agent(Bandit, learner=clf, policy=policy):
-    arm1 = Arm(action1_func, reward_func)
-    arm2 = Arm(action2_func, reward_func)
+    arm1 = Arm("action 1", reward_func)
+    arm2 = Arm("action 2", reward_func)
 
 agent = Agent()
 
 agent.pull() # receive some reward
 agent.update("yes") # update with observed reward
 
 ```
@@ -40,8 +32,8 @@
 
 ```
 pip install -U bayesianbandits
 ```
 
 ## Usage
 
-Check out the [documentation](https://bayesianbandits.readthedocs.io/en/latest/) for examples and an API reference. 
+Check out the [documentation](https://bayesianbandits.readthedocs.io/en/latest/) for examples and an API reference.
```

### Comparing `bayesianbandits-0.2.5/bayesianbandits/__init__.py` & `bayesianbandits-0.3.0/bayesianbandits/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.2.5/bayesianbandits/_arm.py` & `bayesianbandits-0.3.0/bayesianbandits/_arm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,123 @@
 from __future__ import annotations
-from typing import Callable, Optional, cast
+from typing import Callable, Dict, Optional, TypeVar, cast, Any
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 
-from ._typing import DecayingLearner, Learner
+from ._typing import DecayingLearner, Learner, ActionToken
+
+
+R = TypeVar("R")
+
+
+def requires_learner(func: Callable[..., R]) -> Callable[..., R]:
+    """Decorator to check if the arm has a learner set."""
+
+    def wrapper(self: Arm, *args: Any, **kwargs: Dict[str, Any]):
+        if self.learner is None:
+            raise ValueError("Learner is not set.")
+        return func(self, *args, **kwargs)
+
+    return wrapper
 
 
 class Arm:
     """Arm of a bandit.
 
     Parameters
     ----------
-    action_function : Callable
-        Nullary function to call when the arm is pulled. Should have
-        either directly produce the reward or have a side effect that
-        eventually produces reward. For example, if the arm represents an action
-        to take in an experiment, the action function should perform the
-        database query to update the experiment table with the action to take.
-        Later, the `update` method should be called with the computed reward.
+    action_token : Any
+        Token to return when the arm is pulled. This should be something processed
+        by the user's code to execute the action associated with the arm.
     reward_function : Callable
         Function to call to compute the reward. Takes the output of the learner's
         `sample` function as input and should return a scalar reward.
     learner : Optional[Learner], default=None
         Learner to use for the arm. If None, the arm cannot be used.
 
     Examples
     --------
     >>> from bayesianbandits import Arm
     >>> import numpy as np
-    >>> def action_function():
-    ...     print("Action taken.")
     >>> def reward_function(sample):
     ...     return sample
     >>> class MyLearner:
     ...     def sample(self, X, size=1):
     ...         np.random.seed(0)
     ...         return np.random.normal(size=size)
     ...     def partial_fit(self, X, y):
     ...         pass
     >>> learner = MyLearner()
-    >>> arm = Arm(action_function, reward_function, learner)
+    >>> arm = Arm("Action taken.", reward_function, learner)
     >>> arm.pull()
-    Action taken.
+    'Action taken.'
     >>> arm.update(1)
 
     """
 
     def __init__(
         self,
-        action_function: Callable[[], None],
+        action_token: Any,
         reward_function: Callable[[ArrayLike], ArrayLike],
         learner: Optional[Learner] = None,
     ) -> None:
-        self.action_function = action_function
+        self.action_token = ActionToken(action_token)
         self.reward_function = reward_function
         self.learner = learner
 
-    def pull(self) -> None:
+    @requires_learner
+    def pull(self) -> ActionToken:
         """Pull the arm."""
-        if self.learner is None:
-            raise ValueError("Learner is not set.")
-        return self.action_function()
+        return self.action_token
 
+    @requires_learner
     def sample(
         self,
         X: Optional[ArrayLike] = None,
         size: int = 1,
     ) -> NDArray[np.float_]:
         """Sample from learner and compute the reward."""
-        if self.learner is None:
-            raise ValueError("Learner is not set.")
         if X is None:
             X_new = np.array([[1]])
         else:
             X_new = np.atleast_2d(X)
 
         return self.reward_function(self.learner.sample(X_new, size))  # type: ignore
 
+    @requires_learner
     def update(self, X: ArrayLike, y: Optional[ArrayLike] = None) -> None:
         """Update the learner.
 
         If y is None, the data in X is used as the target and X is set to
         a `len(X)` rows of ones.
         """
-        if self.learner is None:
-            raise ValueError("Learner is not set.")
+
         if y is None:
             y_fit = np.atleast_1d(X)
             X_fit = np.ones_like(y_fit, dtype=np.float64)[:, np.newaxis]
         else:
             y_fit, X_fit = np.atleast_1d(y), np.atleast_2d(X)
 
+        assert self.learner is not None  # for type checker
         self.learner.partial_fit(X_fit, y_fit)
 
-    def decay(self, X: ArrayLike, y: Optional[ArrayLike] = None) -> None:
+    @requires_learner
+    def decay(
+        self,
+        X: NDArray[np.float_],
+        *,
+        decay_rate: Optional[float] = None,
+    ) -> None:
         """Decay the learner.
 
         Takes a `y` argument for consistency with `update` but does not use it."""
-        if self.learner is None:
-            raise ValueError("Learner is not set.")
         if not hasattr(self.learner, "decay"):
             raise ValueError("Learner does not have a decay method.")
-        if y is None:
-            y_fit = np.atleast_1d(X)
-            X_fit = np.ones_like(y_fit, dtype=np.float64)[:, np.newaxis]
-        else:
-            y_fit, X_fit = np.atleast_1d(y), np.atleast_2d(X)
 
-        cast(DecayingLearner, self.learner).decay(X_fit)
+        cast(DecayingLearner, self.learner).decay(X, decay_rate=decay_rate)
 
     def __repr__(self) -> str:
         return (
-            f"Arm(action_function={self.action_function},"
+            f"Arm(action_token={self.action_token},"
             f" reward_function={self.reward_function}"
         )
```

### Comparing `bayesianbandits-0.2.5/bayesianbandits/_basebandit.py` & `bayesianbandits-0.3.0/bayesianbandits/_basebandit.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,31 +18,34 @@
 import numpy as np
 from numpy.typing import ArrayLike
 from sklearn.base import clone
 from typing_extensions import dataclass_transform
 
 from ._typing import ArmProtocol, BanditProtocol, Learner
 
+
 _B = TypeVar("_B", bound="Bandit")
 
 
-@dataclass_transform(field_specifiers=(Field, field))
+@dataclass_transform(field_specifiers=(Field[Any], field))
 @dataclass
 class Bandit:
     """
     Base class for bandits. This class is not meant to be instantiated directly.
     Instead, it should be subclassed and the `learner` and `policy` arguments to
     the `__init_subclass__` method should be set. Optionally, the `delayed_reward`
     argument can be set to `True` to enable delayed rewards.
 
-    By default, `Bandit` subclasses take the following arguments to their
-    `__init__` method:
+    Subclass parameters should be passed to `__init_subclass__` during
+    subclassing as keyword arguments. These parameters will be added to
+    the subclass as class attributes.
 
     Subclass Parameters
     -------------------
+
     learner : Learner
         Learner underlying each arm. Must implement `partial_fit` and `sample`.
     policy : Callable[..., ArmProtocol]
         Policy for choosing arms. Must take a `Bandit` instance as its first
         argument and return an `ArmProtocol` instance.
     delayed_reward : bool, optional
         Whether or not rewards are measured between pulls, by default False.
@@ -80,46 +83,44 @@
     `__init_subclass__`. Additionally, all subclasses must define some
     `ArmProtocol` instances as class attributes. These will be used to
     initialize the arms of the bandit.
 
     >>> from bayesianbandits import Arm, GammaRegressor, epsilon_greedy
     >>> clf = GammaRegressor(alpha=1, beta=1)
     >>> policy = epsilon_greedy(0.1)
-    >>> def action_func():
-    ...     print("Action!")
     >>> def reward_func(x):
     ...     return x
     >>> class MyBandit(Bandit, learner=clf, policy=policy):
-    ...     arm1 = Arm(action_func, reward_func)
-    ...     arm2 = Arm(action_func, reward_func)
-    >>> bandit = MyBandit()
+    ...     arm1 = Arm("Action 1!", reward_func)
+    ...     arm2 = Arm("Action 2!", reward_func)
+    >>> bandit = MyBandit(rng=0)
 
     Once subclassed and instantiated, the `pull` method can be used to pull
     arms. For non-contextual bandits, the `pull` method takes no arguments.
     After pulling an arm, the `update` method can be used to update the
     learner underlying the arm.
 
     >>> bandit.pull()
-    Action!
+    'Action 1!'
     >>> bandit.update(1)
 
     For delayed reward bandits, the subclass must set the `delayed_reward`
     argument to `__init_subclass__` to `True`.
 
     >>> class MyDelayedBandit(Bandit, learner=clf, policy=policy, delayed_reward=True):
-    ...     arm1 = Arm(action_func, reward_func)
-    ...     arm2 = Arm(action_func, reward_func)
-    >>> bandit = MyDelayedBandit(cache={})
+    ...     arm1 = Arm("Action 1!", reward_func)
+    ...     arm2 = Arm("Action 2!", reward_func)
+    >>> bandit = MyDelayedBandit(cache={}, rng=0)
 
     When `delayed_reward` is set to `True`, the `pull` method takes an additional
     argument, `unique_id`, which is used to identify the arm pulled. This is
     used to retrieve the arm from the `cache` when the `update` method is called.
 
     >>> bandit.pull(unique_id=1)
-    Action!
+    'Action 1!'
     >>> bandit.update(1, unique_id=1)
 
     """
 
     rng: Union[np.random.Generator, None, int] = field(default=None, repr=False)
     last_arm_pulled: Optional[ArmProtocol] = field(default=None, init=False, repr=False)
     cache: Optional[MutableMapping[Any, str]] = field(default=None, repr=False)
@@ -130,15 +131,15 @@
 
     def __init_subclass__(
         cls,
         /,
         learner: Learner,
         policy: Callable[..., ArmProtocol],
         delayed_reward: bool = False,
-        **kwargs,
+        **kwargs: Dict[str, Any],
     ):
         """Initialize a subclass of `Bandit`.
 
         Parameters
         ----------
         learner : Learner
             Learner to use for each arm.
@@ -160,58 +161,59 @@
             setattr(cls, "cache", field(default=None, init=False, repr=False))
 
         # make sure cache is annotated for dataclass magic
         annotations: dict[str, Any] = getattr(cls, "__annotations__", {})
         annotations["cache"] = Optional[MutableMapping[Any, ArmProtocol]]
 
         # collect and annotate all ArmProtocol instances
-        arm_annotations = {}
+        arm_annotations: Dict[str, Any] = {}
 
         for name, attr in cls.__dict__.items():
             if isinstance(attr, ArmProtocol):
                 arm_annotations[name] = ArmProtocol
                 setattr(
                     cls,
                     name,
                     field(default_factory=partial(deepcopy, attr), init=False),
                 )
 
         # make sure all ArmProtocol instances are first in the annotations
         # for dataclass magic - this is unnecessary in Python 3.10
-        arm_annotations.update(
-            {k: v for k, v in annotations.items() if k not in arm_annotations}
-        )
+        other_annotations = {
+            k: v for k, v in annotations.items() if k not in arm_annotations
+        }
+        arm_annotations.update(other_annotations)
 
         setattr(cls, "__annotations__", arm_annotations)
 
         # modifies cls in-place
         dataclass(cls)
 
     @overload
-    def pull(self, X: ArrayLike, /) -> None:
+    def pull(self, X: ArrayLike, /) -> Any:
         ...
 
     @overload
-    def pull(self, X: ArrayLike, /, *, unique_id: Any) -> None:
+    def pull(self, X: ArrayLike, /, *, unique_id: Any) -> Any:
         ...
 
     @overload
-    def pull(self, /) -> None:
+    def pull(self, /) -> Any:
         ...
 
     @overload
-    def pull(self, /, *, unique_id: Any) -> None:
+    def pull(self, /, *, unique_id: Any) -> Any:
         ...
 
     def pull(
         self,
         X: Optional[ArrayLike] = None,
         /,
         **kwargs: Any,
-    ) -> None:
+    ) -> Any:
         """Choose an arm and pull it. Set `last_arm_pulled` to the name of the
         arm that was pulled.
 
         This method is added to the bandit class by the `bandit` decorator.
 
         Parameters
         ----------
@@ -229,27 +231,31 @@
         if X is None and self._contextual:
             raise ValueError("X must be an array-like for a contextual bandit.")
         elif X is not None and not self._contextual:
             raise ValueError("X must be None for a non-contextual bandit.")
 
         arm = self.policy(X)
         self.last_arm_pulled = arm
+        unique_id = None
 
         if self.__class__._delayed_reward is True:
             unique_id = kwargs.get("unique_id")
             if unique_id is None:
                 raise ValueError(
                     "The `unique_id` keyword argument is required when the "
                     "`delayed_reward = True`."
                 )
 
         ret_val = arm.pull()
 
         if self.__class__._delayed_reward is True:
-            (self.cache[unique_id],) = [  # type: ignore
+            # this is here for the type checker
+            assert self.cache is not None
+
+            (self.cache[unique_id],) = [
                 k for k, v in self.arms.items() if v is self.last_arm_pulled
             ]
 
         return ret_val
 
     @overload
     def update(self, y: ArrayLike, /) -> None:
@@ -264,19 +270,15 @@
         ...
 
     @overload
     def update(self, X: ArrayLike, y: ArrayLike, /, *, unique_id: Any) -> None:
         ...
 
     def update(
-        self,
-        X: ArrayLike,
-        y: Optional[ArrayLike] = None,
-        /,
-        **kwargs: Any,
+        self, X: ArrayLike, y: Optional[ArrayLike] = None, /, **kwargs: Dict[str, Any]
     ) -> None:
         """Update the learner for the last arm pulled.
 
         This method is added to the bandit class by the `bandit` decorator.
 
         Parameters
         ----------
@@ -356,14 +358,57 @@
         elif X is not None and not self._contextual:
             raise ValueError("X must be None for a non-contextual bandit.")
         # choose an arm, draw a sample, and repeat `size` times
         # TODO: this is not the most efficient way to do this
         # but I can't imagine a situation where this would be a bottleneck.
         return np.array([self.policy(X).sample(X) for _ in range(size)])
 
+    @overload
+    def decay(self, /, *, decay_last_arm: bool = True) -> None:
+        ...
+
+    @overload
+    def decay(self, X: ArrayLike, /, *, decay_last_arm: bool = True) -> None:
+        ...
+
+    def decay(
+        self,
+        X: Optional[ArrayLike] = None,
+        /,
+        *,
+        decay_rate: Optional[float] = None,
+        decay_last_arm: bool = True,
+    ) -> None:
+        """Decay the all arms in the bandit.
+
+        Optionally, decay the last arm pulled.
+
+        Parameters
+        ----------
+        X : Optional[ArrayLike]
+            Context for the bandit. Only provided when the @contextual
+            decorator is used.
+        decay_last_arm : bool, default=True
+            Whether to decay the last arm pulled.
+        """
+        if X is None and self._contextual:
+            raise ValueError("X must be an array-like for a contextual bandit.")
+        elif X is not None and not self._contextual:
+            raise ValueError("X must be None for a non-contextual bandit.")
+
+        if not self._contextual:
+            X_decay = np.array([[1]])
+        else:
+            assert X is not None  # for the type checker
+            X_decay = np.atleast_2d(X)
+
+        for arm in self.arms.values():
+            if decay_last_arm or arm is not self.last_arm_pulled:
+                arm.decay(X_decay, decay_rate=decay_rate)
+
     def __post_init__(self) -> None:
         """Moves all class attributes that are instances of `Arm` to instance
         attributes.
 
         This ensures that the bandit can be pickled."""
 
         self.rng = np.random.default_rng(self.rng)
@@ -403,15 +448,15 @@
         ]
 
         for arm_name in to_del:
             del self.arms[arm_name]
             del self.__dict__[arm_name]
 
         # initialize arms that are newly defined
-        for arm_name, arm in currently_defined_arms.items():
+        for arm_name, _ in currently_defined_arms.items():
             if arm_name not in self.arms:
                 new_arm = self.__class__.__dataclass_fields__[
                     arm_name
                 ].default_factory()
                 new_arm.learner = cast(Learner, clone(self.learner))  # type: ignore
                 setattr(self, arm_name, new_arm)  # type: ignore
                 self.arms[arm_name] = self.__dict__[arm_name]
@@ -449,39 +494,37 @@
 
     A contextual bandit can be created by decorating a Bandit subclass with
     the `contextual` decorator.
 
     >>> from bayesianbandits import Arm, GammaRegressor, epsilon_greedy
     >>> clf = GammaRegressor(alpha=1, beta=1)
     >>> policy = epsilon_greedy(0.1)
-    >>> def action_func():
-    ...     print("Action!")
     >>> def reward_func(x):
     ...     return x
     >>> @contextual
     ... class MyBandit(Bandit, learner=clf, policy=policy):
-    ...     arm1 = Arm(action_func, reward_func)
-    ...     arm2 = Arm(action_func, reward_func)
-    >>> bandit = MyBandit()
+    ...     arm1 = Arm("Action 1!", reward_func)
+    ...     arm2 = Arm("Action 2!", reward_func)
+    >>> bandit = MyBandit(rng=0)
 
     The `pull`, `sample`, and `update` methods now take an `X` argument.
 
     >>> bandit.pull(1)
-    Action!
+    'Action 1!'
     >>> bandit.update(1, 1)
 
     """
 
     check_is_bandit(cls)
 
-    orig_post_init = cls.__post_init__  # type: ignore
+    orig_post_init = cls.__post_init__
 
-    def _contextual_post_init(self) -> None:
+    def _contextual_post_init(self: _B) -> None:
         orig_post_init(self)
-        self._contextual = True
+        self._contextual = True  # type: ignore
 
     setattr(cls, "__post_init__", _contextual_post_init)
 
     return cls
 
 
 def restless(
@@ -502,19 +545,21 @@
     def _restless_update(
         self: Bandit,
         X: ArrayLike,
         y: Optional[ArrayLike] = None,
         **kwargs: ArrayLike,
     ) -> None:
         orig_update(self, X, y, **kwargs)  # type: ignore
-        for arm in self.arms.values():
-            if arm is not self.last_arm_pulled:
-                arm.decay(X, y)
+
+        if self._contextual:  # type: ignore
+            self.decay(X, decay_last_arm=False)
+        else:
+            self.decay(decay_last_arm=False)
 
     setattr(cls, "update", _restless_update)
 
     return cast(Type[_B], cls)
 
 
-def check_is_bandit(cls):
+def check_is_bandit(cls: type):
     if not issubclass(cls, Bandit):
         raise ValueError("This decorator can only be used on a Bandit subclass.")
```

### Comparing `bayesianbandits-0.2.5/bayesianbandits/_estimators.py` & `bayesianbandits-0.3.0/bayesianbandits/_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from collections import defaultdict
 from functools import partial
-from typing import Any, Dict, Union, cast
+from typing import Any, Dict, Optional, Union, cast
 
 import numpy as np
 from numpy.typing import NDArray, ArrayLike
 from scipy.linalg import solve
 from scipy.stats import dirichlet, gamma, multivariate_normal, multivariate_t
 from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin  # type: ignore
 from sklearn.utils.validation import check_array  # type: ignore
@@ -204,22 +204,26 @@
                 list(
                     dirichlet.rvs(alpha, size, self.random_state_)  # type: ignore
                     for alpha in alphas
                 ),
             )
         )
 
-    def decay(self, X: NDArray[Any]) -> None:
+    def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         """
         Decay the prior by a factor of `learning_rate`.
         """
         if not hasattr(self, "known_alphas_"):
             self._initialize_prior()
+
+        if decay_rate is None:
+            decay_rate = self.learning_rate
+
         for x in X:
-            self.known_alphas_[x.item()] *= self.learning_rate
+            self.known_alphas_[x.item()] *= decay_rate
 
 
 class GammaRegressor(BaseEstimator, RegressorMixin):
     """
     Intercept-only Gamma regression model.
 
     Parameters
@@ -390,22 +394,26 @@
 
         return np.squeeze(
             np.stack(
                 list(rv_gen(alpha, scale=1 / beta) for alpha, beta in shape_params),
             )
         )
 
-    def decay(self, X: NDArray[Any]) -> None:
+    def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         """
         Decay the prior by a factor of `learning_rate`.
         """
         if not hasattr(self, "coef_"):
             self._initialize_prior()
+
+        if decay_rate is None:
+            decay_rate = self.learning_rate
+
         for x in X:
-            self.coef_[x.item()] *= self.learning_rate
+            self.coef_[x.item()] *= decay_rate
 
 
 class NormalRegressor(BaseEstimator, RegressorMixin):
     """
     A Bayesian linear regression model that assumes a Gaussian noise distribution.
 
     Parameters
@@ -598,22 +606,25 @@
         samples = np.atleast_1d(rv_gen(self.coef_, cov))  # type: ignore
 
         if self.n_features_ == 1:
             samples = np.expand_dims(samples, -1)
 
         return np.atleast_2d(samples @ X.T)  # type: ignore
 
-    def decay(self, X: NDArray[Any]) -> None:
+    def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         """
         Decay the prior by a factor of `learning_rate`.
         """
         if not hasattr(self, "coef_"):
             self._initialize_prior(X)
 
-        prior_decay = self.learning_rate ** len(X)
+        if decay_rate is None:
+            decay_rate = self.learning_rate
+
+        prior_decay = decay_rate ** len(X)
 
         # Decay the prior without making an update. Because we're only
         # increasing the prior variance, we do not need to update the
         # mean.
         cov_inv = prior_decay * self.cov_inv_
 
         self.cov_inv_ = cov_inv
@@ -817,26 +828,29 @@
 
         samples = np.atleast_1d(rv_gen(self.coef_, shape, df))  # type: ignore
         if self.n_features_ == 1:
             samples = np.expand_dims(samples, -1)
 
         return np.atleast_2d(samples @ X.T)  # type: ignore
 
-    def decay(self, X: NDArray[Any]):
+    def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         """
         Decay the prior by a factor of `learning_rate`. This is equivalent to
         applying the learning rate to the prior, and then ignoring the data.
         It does not change the mean of the coefficient marginal posterior, but
         it does increase the variance.
         """
 
         if not hasattr(self, "coef_"):
             self._initialize_prior(X)
 
-        prior_decay = self.learning_rate ** len(X)
+        if decay_rate is None:
+            decay_rate = self.learning_rate
+
+        prior_decay = decay_rate ** len(X)
 
         # decay only increases the variance, so we only need to update the
         # inverse covariance matrix, a_, and b_
         V_n = prior_decay * self.cov_inv_
 
         a_n = prior_decay * self.a_
```

### Comparing `bayesianbandits-0.2.5/bayesianbandits/_np_utils.py` & `bayesianbandits-0.3.0/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.2.5/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.3.0/bayesianbandits/_policy_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,28 +141,28 @@
 
 
 def _compute_arm_upper_bound(
     arm: ArmProtocol,
     X: Optional[ArrayLike] = None,
     *,
     alpha: float = 0.68,
-    samples=1000,
+    samples: int = 1000,
 ) -> np.float_:
     """Compute the upper bound of a one-sided credible interval with size
     `alpha` from the posterior distribution for the arm."""
     posterior_samples = arm.sample(X, size=samples)
     posterior_samples = cast(NDArray[np.float64], posterior_samples)
 
     return np.quantile(posterior_samples, q=alpha)  # type: ignore
 
 
 def _compute_arm_mean(
     arm: ArmProtocol,
     X: Optional[ArrayLike] = None,
     *,
-    samples=1000,
+    samples: int = 1000,
 ) -> np.float_:
     """Compute the mean of the posterior distribution for the arm."""
     posterior_samples = arm.sample(X, size=samples)
     posterior_samples = cast(NDArray[np.float64], posterior_samples)
 
     return np.mean(posterior_samples)
```

### Comparing `bayesianbandits-0.2.5/bayesianbandits/_typing.py` & `bayesianbandits-0.3.0/bayesianbandits/_typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from __future__ import annotations
-from typing import Any, Callable, Dict, Optional, Protocol, Union, runtime_checkable
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    NewType,
+    Optional,
+    Protocol,
+    Union,
+    runtime_checkable,
+)
 
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 
+ActionToken = NewType("TokenType", Any)
+
 
 class Learner(Protocol):
     """Learner protocol for the model underlying each arm.
 
     Each Learner must implement the following methods:
     - `sample`
     - `partial_fit`
@@ -29,44 +40,50 @@
     def set_params(self, **params: Any) -> "Learner":
         ...
 
 
 class DecayingLearner(Learner, Protocol):
     learning_rate: float
 
-    def decay(self, X: NDArray[Any]) -> None:
+    def decay(self, X: NDArray[Any], *, decay_rate: Optional[float] = None) -> None:
         ...
 
 
 @runtime_checkable
 class ArmProtocol(Protocol):
     """Protocol for Arms and Bandits. Bandits themselves can be used as arms
     in other bandits, so both must implement the same minimal interface.
 
     Each Arm or Bandit must implement the following methods:
     - `pull`
     - `sample`
     - `update`
+    - `decay`
 
     """
 
     learner: Optional[Learner]
 
-    def pull(self) -> None:
+    def pull(self) -> ActionToken:
         ...
 
     def sample(
         self, X: Optional[ArrayLike] = None, size: int = 1
     ) -> NDArray[np.float_]:
         ...
 
     def update(self, X: ArrayLike, y: Optional[ArrayLike] = None) -> None:
         ...
 
-    def decay(self, X: ArrayLike, y: Optional[ArrayLike] = None) -> None:
+    def decay(
+        self,
+        X: NDArray[np.float_],
+        *,
+        decay_rate: Optional[float] = None,
+    ) -> None:
         ...
 
 
 @runtime_checkable
 class BanditProtocol(Protocol):
     """Protocol for Bandits.
 
@@ -85,15 +102,15 @@
     _contextual: bool
 
     def __init__(
         *args: Any, rng: Union[np.random.Generator, int, None] = None, **kwargs: Any
     ) -> None:
         ...
 
-    def pull(self, X: Optional[ArrayLike] = None, **kwargs: Any) -> None:
+    def pull(self, X: Optional[ArrayLike] = None, **kwargs: Any) -> ActionToken:
         ...
 
     def sample(
         self, X: Optional[ArrayLike] = None, size: int = 1, **kwargs: Any
     ) -> ArrayLike:
         ...
```

### Comparing `bayesianbandits-0.2.5/pyproject.toml` & `bayesianbandits-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.2.5"
+version = "0.3.0"
 description = ""
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
```

### Comparing `bayesianbandits-0.2.5/PKG-INFO` & `bayesianbandits-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,28 +24,20 @@
 import numpy as np
 
 from bayesianbandits import Bandit, Arm, epsilon_greedy, DirichletClassifier
 
 def reward_func(x):
     return np.take(x, 0, axis=-1)
 
-def action1_func():
-    # do action 1
-    ...
-
-def action2_func():
-    # do action 2
-    ...
-
 clf = DirichletClassifier({"yes": 1.0, "no": 1.0})
 policy = epsilon_greedy(0.1)
 
 class Agent(Bandit, learner=clf, policy=policy):
-    arm1 = Arm(action1_func, reward_func)
-    arm2 = Arm(action2_func, reward_func)
+    arm1 = Arm("action 1", reward_func)
+    arm2 = Arm("action 2", reward_func)
 
 agent = Agent()
 
 agent.pull() # receive some reward
 agent.update("yes") # update with observed reward
 
 ```
@@ -56,8 +48,9 @@
 
 ```
 pip install -U bayesianbandits
 ```
 
 ## Usage
 
-Check out the [documentation](https://bayesianbandits.readthedocs.io/en/latest/) for examples and an API reference. 
+Check out the [documentation](https://bayesianbandits.readthedocs.io/en/latest/) for examples and an API reference.
+
```

