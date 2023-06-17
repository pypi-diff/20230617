# Comparing `tmp/onion_config-1.0.1.tar.gz` & `tmp/onion_config-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_config-1.0.1.tar", last modified: Sun Jul 31 07:58:53 2022, max compression
+gzip compressed data, was "onion_config-2.0.0.tar", last modified: Sat Jun 17 07:39:19 2023, max compression
```

## Comparing `onion_config-1.0.1.tar` & `onion_config-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 07:58:53.821109 onion_config-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-31 07:58:42.000000 onion_config-1.0.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6755 2022-07-31 07:58:53.821109 onion_config-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-07-31 07:58:42.000000 onion_config-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 07:58:53.821109 onion_config-1.0.1/onion_config/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-31 07:58:42.000000 onion_config-1.0.1/onion_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-31 07:58:42.000000 onion_config-1.0.1/onion_config/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10967 2022-07-31 07:58:42.000000 onion_config-1.0.1/onion_config/config_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 07:58:53.821109 onion_config-1.0.1/onion_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6755 2022-07-31 07:58:53.000000 onion_config-1.0.1/onion_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-31 07:58:53.000000 onion_config-1.0.1/onion_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-31 07:58:53.000000 onion_config-1.0.1/onion_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-07-31 07:58:53.000000 onion_config-1.0.1/onion_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-31 07:58:53.000000 onion_config-1.0.1/onion_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-31 07:58:53.825109 onion_config-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-07-31 07:58:42.000000 onion_config-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:39:19.488968 onion_config-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-17 07:39:02.000000 onion_config-2.0.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-17 07:39:19.488968 onion_config-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-17 07:39:02.000000 onion_config-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:39:19.488968 onion_config-2.0.0/onion_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 07:39:02.000000 onion_config-2.0.0/onion_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 07:39:02.000000 onion_config-2.0.0/onion_config/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14574 2023-06-17 07:39:02.000000 onion_config-2.0.0/onion_config/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:39:19.488968 onion_config-2.0.0/onion_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-06-17 07:39:19.000000 onion_config-2.0.0/onion_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-17 07:39:19.000000 onion_config-2.0.0/onion_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:39:19.000000 onion_config-2.0.0/onion_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-17 07:39:19.000000 onion_config-2.0.0/onion_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 07:39:19.000000 onion_config-2.0.0/onion_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 07:39:19.488968 onion_config-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-17 07:39:02.000000 onion_config-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:39:19.488968 onion_config-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-17 07:39:02.000000 onion_config-2.0.0/tests/test_onion_config.py
```

### Comparing `onion_config-1.0.1/LICENCE.txt` & `onion_config-2.0.0/LICENCE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 MIT License
-Copyright (c) 2022 Batkhuu Byambajav
+
+Copyright (c) 2023 Batkhuu Byambajav
+
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
+
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `onion_config-1.0.1/onion_config/config_base.py` & `onion_config-2.0.0/onion_config/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,297 +1,389 @@
 # -*- coding: utf-8 -*-
 
 import os
 import glob
 import json
 import logging
-import pprint
+from typing import Union, List, Callable, TypeVar
 
 import yaml
 from box import Box
 from dotenv import load_dotenv
-from cerberus import Validator
+from pydantic import BaseSettings, BaseModel, validate_arguments
+from pydantic.env_settings import SettingsSourceCallable
 
 from .__version__ import __version__
 
+
 logger = logging.getLogger(__name__)
 
 
-class ConfigBase:
-    """A core class of 'onion_python' module to use as the base configuration.
+class BaseConfig(BaseSettings):
+    class Config:
+        extra = "allow"
+        frozen = True
+        arbitrary_types_allowed = True
+
+        @classmethod
+        def customise_sources(
+            cls,
+            init_settings: SettingsSourceCallable,
+            env_settings: SettingsSourceCallable,
+            file_secret_settings: SettingsSourceCallable,
+        ) -> tuple[SettingsSourceCallable, ...]:
+            return env_settings, init_settings, file_secret_settings
 
-    Attributes:
-        _CONFIGS_DIR  (str     ): Default configs directory. Defaults to '${PWD}/configs'.
-        _PRE_LOAD     (function): Default lambda function for 'pre_load'. Defaults to <lambda config: config>.
 
-        configs_dir   (str     ): Main configs directory to load all config files. Defaults to _CONFIGS_DIR.
-        required_envs (str     ): Required environment variables to check. Defaults to []
-        valid_schema  (dict    ): Validation schema to validate 'config'. This schema is based on 'Cerberus' package. Defaults to None.
-        config        (box.Box ): Main 'config' object based on 'python-box' package. Defaults to Box().
+_ConfigType = TypeVar("_ConfigType", bound=Union[BaseConfig, BaseSettings, BaseModel])
+
+
+class ConfigLoader:
+    """A core class of 'onion_config' module to use as the main config loader.
+
+    Attributes:
+        _ENV_FILE_PATH    (str     ): Default '.env' file path to load. Defaults to '${PWD}/.env'.
+        _CONFIGS_DIR      (str     ): Default configs directory. Defaults to '${PWD}/configs'.
+        _PRE_LOAD_HOOK    (function): Default lambda function for 'pre_load_hook'. Defaults to <lambda config_data: config_data>.
+
+        config            (Union[BaseConfig, BaseSettings, BaseModel]): Main config object (config_schema) for project. Defaults to None.
+        config_schema     (_ConfigType): Main config schema class to load and validate configs. Defaults to BaseConfig.
+        config_data       (box.Box    ): Loaded data from config files as a 'python-box' Box. Defaults to Box().
+        configs_dir       (str        ): Main configs directory to load all config files. Defaults to ConfigLoader._CONFIGS_DIR.
+        extra_configs_dir (str        ): Extra configs directory to load extra config files. Defaults to None, but will use the 'PY_EXTRA_CONFIGS_DIR' environment variable if set.
+        required_envs     (str        ): Required environment variables to check. Defaults to [].
+        pre_load_hook     (function   ): Custom pre-load method, this method will executed before loading and validating 'config'. Defaults to ConfigLoader._PRE_LOAD_HOOK.
 
     Methods:
-        set_pre_load()         : Setting method for custom 'pre_load' method.
-        load()                 : Load and validate every configs into 'config'.
-        _load_dotenv()         : Loading environment variables from .env file, if it's exits.
-        _check_required_envs() : Check required environment variables are exist or not.
-        _load_config_files()   : Load config files from 'config_dir' into 'config'.
-        _load_extra_configs()  : Load extra config files from 'PY_EXTRA_CONFIGS_DIR' into 'config'.
-        _pre_load()            : Custom pre-load method, this method will executed before validating 'config'. Defaults to ConfigBase._PRE_LOAD.
-        _validate()            : Validate the 'config' by 'valid_schema'.
-        _freeze_config()       : Freeze 'config' into immutable variable.
+        load()                    : Load and validate every configs into 'config'.
+        _load_dotenv()            : Loading environment variables from .env file, if it's exits.
+        _check_required_envs()    : Check required environment variables are exist or not.
+        _load_config_files()      : Load config files from 'configs_dir' into 'config_data'.
+        _load_extra_config_files(): Load extra config files from 'PY_EXTRA_CONFIGS_DIR' into 'config_data'.
     """
 
-    _CONFIGS_DIR = os.path.join(os.getcwd(), 'configs')
-    _PRE_LOAD = lambda config: config
-
-    def __init__(self, configs_dir: str=_CONFIGS_DIR, required_envs: list=[], pre_load: callable=_PRE_LOAD, valid_schema: dict=None):
-        """ConfigBase constructor method.
+    _ENV_FILE_PATH = os.path.join(os.getcwd(), ".env")
+    _CONFIGS_DIR = os.path.join(os.getcwd(), "configs")
+    _PRE_LOAD_HOOK = lambda config_data: config_data
+
+    def __init__(
+        self,
+        configs_dir: str = _CONFIGS_DIR,
+        config_schema: _ConfigType = BaseConfig,
+        required_envs: List[str] = [],
+        pre_load_hook: Callable = _PRE_LOAD_HOOK,
+        env_file_path: str = _ENV_FILE_PATH,
+        extra_configs_dir: Union[str, None] = None,
+        auto_load: bool = False,
+    ):
+        """ConfigLoader constructor method.
 
         Args:
-            configs_dir   (str,      optional): Main configs directory to load all config files. Defaults to ConfigBase._CONFIGS_DIR.
-            required_envs (list,     optional): Required environment variables to check. Defaults to [].
-            pre_load      (function, optional): Custom pre-load method, this method will executed before validating 'config'. Defaults to ConfigBase._PRE_LOAD.
-            valid_schema  (dict,     optional): Validation schema to validate 'config'. This schema is based on 'Cerberus' package. Defaults to None.
+            configs_dir       (str,         optional): Main configs directory to load all config files. Defaults to ConfigLoader._CONFIGS_DIR.
+            config_schema     (_ConfigType, optional): Main config schema class to load and validate configs. Defaults to BaseConfig.
+            required_envs     (list,        optional): Required environment variables to check. Defaults to [].
+            pre_load_hook     (function,    optional): Custom pre-load method, this method will executed before loading and validating 'config'. Defaults to ConfigLoader._PRE_LOAD_HOOK.
+            extra_configs_dir (str,         optional): Extra configs directory to load extra config files. Defaults to None.
+            auto_load         (bool,        optional): Auto load configs on init or not. Defaults to False.
         """
 
         self.configs_dir = configs_dir
+        self.config_schema = config_schema
         self.required_envs = required_envs
-        if valid_schema:
-            self.valid_schema = valid_schema
-        self.set_pre_load(pre_load)
-
-        self.config = Box()
-
+        self.pre_load_hook = pre_load_hook
+        self.env_file_path = env_file_path
+        if extra_configs_dir:
+            self.extra_configs_dir = extra_configs_dir
+        self.config_data = Box()
 
-    def set_pre_load(self, pre_load: callable=_PRE_LOAD):
-        """Setting method for custom 'pre_load' method.
-
-        Args:
-            pre_load (function, optional): Custom pre-load method, this method will executed before validating 'config'. Defaults to ConfigBase._PRE_LOAD.
+        if auto_load:
+            self.load()
 
-        Raises:
-            TypeError: If 'pre_load' argument type is not callable function.
-        """
-
-        if callable(pre_load):
-            self._pre_load = pre_load
-        else:
-            try:
-                raise TypeError(f"'pre_load' argument type <{type(pre_load).__name__}> is invalid, should be callable <function>!")
-            except TypeError as err:
-                logger.exception(err)
-                exit(2)
-
-
-    def load(self):
+    def load(self) -> Union[BaseConfig, BaseSettings, BaseModel]:
         """Load and validate every configs into 'config'.
 
         Returns:
-            Box(): Returns loaded config as a 'python-box' Box().
+            Union[BaseConfig, BaseSettings, BaseModel]: Main config object (config_schema) for project.
         """
 
         self._load_dotenv()
         self._check_required_envs()
         self._load_config_files()
-        self._load_extra_configs()
-        self.config = self._pre_load(self.config)
-        if self.valid_schema:
-            self._validate()
-        self._freeze_config()
-        return self.config
+        self._load_extra_config_files()
 
+        try:
+            self.config_data: Box = self.pre_load_hook(self.config_data)
+        except Exception:
+            logger.critical("Failed to execute 'pre_load_hook' method:")
+            raise
 
-    def _load_dotenv(self):
-        """Loading environment variables from .env file, if it's exits.
-        """
+        try:
+            self.config: Union[
+                BaseConfig, BaseSettings, BaseModel
+            ] = self.config_schema(**self.config_data.to_dict())
+        except Exception:
+            logger.critical("Failed to init 'config_schema':")
+            raise
 
-        _env_filename = '.env'
-        _env_file_path = os.path.join(os.getcwd(), _env_filename)
-        if os.path.isfile(_env_file_path):
-            load_dotenv(dotenv_path=_env_file_path, override=True, encoding='utf8')
+        return self.config
+
+    def _load_dotenv(self):
+        """Loading environment variables from .env file, if it's exits."""
 
+        if os.path.isfile(self.env_file_path):
+            load_dotenv(dotenv_path=self.env_file_path, override=True, encoding="utf8")
 
     def _check_required_envs(self):
-        """Check required environment variables are exist or not.
+        """Check if required environment variables exist or not.
+
+        If a required environment variable does not exist, an error is logged and the program is terminated with 'exit(2)'.
         """
 
         for _env in self.required_envs:
             try:
                 os.environ[_env]
             except KeyError:
-                logger.exception(f"Missing required '{_env}' environment variable.")
-                exit(2)
-
-
-    def _load_config_files(self):
-        """Load config files from 'config_dir' into 'config'.
-        """
-
-        ## Loading all JSON config files from 'configs' directory:
-        _json_file_paths = glob.glob(os.path.join(self.configs_dir, '*.json'))
-        for _json_file_path in _json_file_paths:
-            try:
-                with open(_json_file_path, "r", encoding='utf8') as _json_file:
-                    self.config.merge_update(Box(json.load(_json_file) or {}))
-            except Exception:
-                logger.exception(f"Failed to load '{_json_file_path}' json config file:")
-                exit(2)
-
-        ## Loading all YAML config files from 'configs' directory:
-        _yaml_file_paths = glob.glob(os.path.join(self.configs_dir, '*.yml'))
-        _yaml_file_paths.extend(glob.glob(os.path.join(self.configs_dir, '*.yaml')))
-        for _yaml_file_path in _yaml_file_paths:
-            try:
-                with open(_yaml_file_path, "r", encoding='utf8') as _yaml_file:
-                    self.config.merge_update(Box(yaml.safe_load(_yaml_file) or {}))
-            except Exception:
-                logger.exception(f"Failed to load '{_yaml_file_path}' yaml config file:")
-                exit(2)
+                logger.critical(f"Missing required '{_env}' environment variable.")
+                raise
 
+    @validate_arguments
+    def _load_config_files(self, configs_dir: Union[str, None] = None):
+        """Load config files from 'configs_dir' into 'config_data'.
 
-    def _load_extra_configs(self):
-        """Load extra config files from 'PY_EXTRA_CONFIGS_DIR' into 'config'.
+        Args:
+            configs_dir (str, optional): Main configs directory to load all config files. Defaults to ConfigLoader._CONFIGS_DIR.
         """
 
-        ## Checking 'PY_EXTRA_CONFIGS_DIR' directory exists, and if it exists, loads config files from that directory:
-        _extra_configs_dir = os.getenv('PY_EXTRA_CONFIGS_DIR')
-        if _extra_configs_dir and os.path.isdir(_extra_configs_dir):
-
-            _json_file_paths = glob.glob(os.path.join(_extra_configs_dir, '*.json'))
+        _configs_dir = self.configs_dir
+        if configs_dir:
+            _configs_dir = configs_dir
+
+        if os.path.isdir(_configs_dir):
+            ## Loading all JSON config files from 'configs' directory:
+            _json_file_paths = sorted(glob.glob(os.path.join(_configs_dir, "*.json")))
             for _json_file_path in _json_file_paths:
                 try:
-                    with open(_json_file_path, "r", encoding='utf8') as _json_file:
-                        self.config.merge_update(Box(json.load(_json_file) or {}))
+                    with open(_json_file_path, "r", encoding="utf8") as _json_file:
+                        self.config_data.merge_update(Box(json.load(_json_file) or {}))
                 except Exception:
-                    logger.exception(f"Failed to load '{_json_file_path}' json config file:")
-                    exit(2)
-
-            _yaml_file_paths = glob.glob(os.path.join(_extra_configs_dir, '*.yml'))
-            _yaml_file_paths.extend(glob.glob(os.path.join(self.configs_dir, '*.yaml')))
+                    logger.critical(
+                        f"Failed to load '{_json_file_path}' json config file:"
+                    )
+                    raise
+
+            ## Loading all YAML config files from 'configs' directory:
+            _yaml_file_paths = glob.glob(os.path.join(_configs_dir, "*.yml"))
+            _yaml_file_paths.extend(glob.glob(os.path.join(_configs_dir, "*.yaml")))
+            _yaml_file_paths.sort()
             for _yaml_file_path in _yaml_file_paths:
                 try:
-                    with open(_yaml_file_path, "r", encoding='utf8') as _yaml_file:
-                        self.config.merge_update(Box(yaml.safe_load(_yaml_file) or {}))
+                    with open(_yaml_file_path, "r", encoding="utf8") as _yaml_file:
+                        self.config_data.merge_update(
+                            Box(yaml.safe_load(_yaml_file) or {})
+                        )
                 except Exception:
-                    logger.exception(f"Failed to load '{_yaml_file_path}' yaml config file:")
-                    exit(2)
+                    logger.critical(
+                        f"Failed to load '{_yaml_file_path}' yaml config file:"
+                    )
+                    raise
+
+    def _load_extra_config_files(self):
+        """Load extra config files from 'PY_EXTRA_CONFIGS_DIR' into 'config_data'."""
+
+        if self.extra_configs_dir is None:
+            _env_extra_configs_dir = os.getenv("PY_EXTRA_CONFIGS_DIR")
+            if _env_extra_configs_dir:
+                self.extra_configs_dir = _env_extra_configs_dir
 
+        if self.extra_configs_dir:
+            self._load_config_files(configs_dir=self.extra_configs_dir)
 
-    def _validate(self):
-        """Validate the 'config' by 'valid_schema'.
-
-        Raises:
-            ValueError: If 'config' is invalid based on 'valid_schema'.
-        """
+    ### ATTRIBUTES ###
 
+    ## config ##
+    @property
+    def config(self) -> Union[BaseConfig, BaseSettings, BaseModel, None]:
         try:
-            _v = Validator(self.valid_schema)
-            _v.allow_unknown = True
-            _v.require_all = True
-            if not _v.validate(self.config.to_dict()):
-                _err_str = "The 'config' is invalid:\n"
-                for _key, _value in _v.errors.items():
-                    _err_str = _err_str + f"'{_key}' field is invalid => {_value}\n"
-                raise ValueError(_err_str)
-
-            self.config = Box(_v.document)
-        except Exception as err:
-            logger.exception(err)
-            exit(2)
+            return self.__config
+        except AttributeError:
+            return None
 
+    @config.setter
+    def config(self, config: Union[BaseConfig, BaseSettings, BaseModel]):
+        if (
+            (not isinstance(config, BaseConfig))
+            and (not isinstance(config, BaseSettings))
+            and (not isinstance(config, BaseModel))
+        ):
+            raise TypeError(
+                f"The 'config' attribute type {type(config)} is invalid, must be a <class 'BaseConfig'> or 'pydantic' <class 'BaseSettings'> or <class 'BaseModel'>."
+            )
 
-    def _freeze_config(self):
-        """Freeze 'config' into immutable variable.
-        """
+        self.__config = config
 
-        self.config = Box(self.config, frozen_box=True)
-        # logger.debug('\n' + pprint.pformat(self.config) + '\n')
+    ## config ##
 
+    ## config_schema ##
+    @property
+    def config_schema(self) -> _ConfigType:
+        try:
+            return self.__config_schema
+        except AttributeError:
+            return BaseConfig
 
-    ### ATTRIBUTES ###
-    ## config ##
+    @config_schema.setter
+    def config_schema(self, config_schema: _ConfigType):
+        # Check if config_schema is a class (i.e., an instance of type)
+        if not isinstance(config_schema, type):
+            raise TypeError("'config_schema' must be a class, not an instance.")
+
+        # Check if config_schema is a subclass of BaseConfig, BaseSettings or BaseModel
+        if (
+            (not issubclass(config_schema, BaseConfig))
+            and (not issubclass(config_schema, BaseSettings))
+            and (not issubclass(config_schema, BaseModel))
+        ):
+            _base_class = ""
+            if hasattr(config_schema, "__base__"):
+                _base_class = config_schema.__base__
+            else:
+                _base_class = type(config_schema)
+
+            raise TypeError(
+                f"The 'config_schema' attribute base class {_base_class} is invalid, must be a Type[<class 'BaseConfig'>] or 'pydantic' Type[<class 'BaseSettings'>, <class 'BaseModel'>]."
+            )
+
+        self.__config_schema = config_schema
+
+    ## config_schema ##
+
+    ## config_data ##
     @property
-    def config(self):
+    def config_data(self) -> Union[Box, None]:
         try:
-            return self.__config
+            return self.__config_data
         except AttributeError:
             return None
 
-    @config.setter
-    def config(self, config):
-        try:
-            if not isinstance(config, Box):
-                raise TypeError(f"The 'config' attribute type <{type(config).__name__}> is invalid, must be a 'python-box' <class 'Box'>.")
-        except TypeError as err:
-            logger.exception(err)
-            exit(2)
+    @config_data.setter
+    def config_data(self, config_data: Box):
+        if not isinstance(config_data, Box):
+            raise TypeError(
+                f"The 'config_data' attribute type {type(config_data)} is invalid, must be a 'python-box' <class 'Box'>."
+            )
 
-        self.__config = config
-    ## config ##
+        self.__config_data = config_data
 
+    ## config_data ##
 
     ## configs_dir ##
     @property
-    def configs_dir(self):
+    def configs_dir(self) -> str:
         try:
             return self.__configs_dir
         except AttributeError:
-            return ConfigBase._CONFIGS_DIR
+            return ConfigLoader._CONFIGS_DIR
 
     @configs_dir.setter
-    def configs_dir(self, configs_dir):
-        try:
-            if not isinstance(configs_dir, str):
-                raise TypeError(f"The 'configs_dir' attribute type <{type(configs_dir).__name__}> is invalid, must be a <str>!")
-
-            configs_dir = configs_dir.strip()
-            if configs_dir == '':
-                raise ValueError("The 'configs_dir' attribute value is empty!")
-        except Exception as err:
-            logger.exception(err)
-            exit(2)
+    def configs_dir(self, configs_dir: str):
+        if not isinstance(configs_dir, str):
+            raise TypeError(
+                f"The 'configs_dir' attribute type {type(configs_dir)} is invalid, must be a <str>!"
+            )
+
+        configs_dir = configs_dir.strip()
+        if configs_dir == "":
+            raise ValueError("The 'configs_dir' attribute value is empty!")
 
         self.__configs_dir = configs_dir
+
     ## configs_dir ##
 
+    ## extra_configs_dir ##
+    @property
+    def extra_configs_dir(self) -> Union[str, None]:
+        try:
+            return self.__extra_configs_dir
+        except AttributeError:
+            return None
+
+    @extra_configs_dir.setter
+    def extra_configs_dir(self, extra_configs_dir: str):
+        if not isinstance(extra_configs_dir, str):
+            raise TypeError(
+                f"The 'extra_configs_dir' attribute type {type(extra_configs_dir)} is invalid, must be a <str>!"
+            )
+
+        extra_configs_dir = extra_configs_dir.strip()
+        if extra_configs_dir == "":
+            raise ValueError("The 'extra_configs_dir' attribute value is empty!")
+
+        self.__extra_configs_dir = extra_configs_dir
+
+    ## extra_configs_dir ##
+
+    ## env_file_path ##
+    @property
+    def env_file_path(self) -> str:
+        try:
+            return self.__env_file_path
+        except AttributeError:
+            return ConfigLoader._ENV_FILE_PATH
+
+    @env_file_path.setter
+    def env_file_path(self, env_file_path: str):
+        if not isinstance(env_file_path, str):
+            raise TypeError(
+                f"The 'env_file_path' attribute type {type(env_file_path)} is invalid, must be a <str>!"
+            )
+
+        env_file_path = env_file_path.strip()
+        if env_file_path == "":
+            raise ValueError("The 'env_file_path' attribute value is empty!")
+
+        self.__env_file_path = env_file_path
+
+    ## env_file_path ##
 
     ## required_envs ##
     @property
-    def required_envs(self):
+    def required_envs(self) -> List[str]:
         try:
             return self.__required_envs
         except AttributeError:
             return []
 
     @required_envs.setter
-    def required_envs(self, required_envs):
-        try:
-            if not isinstance(required_envs, list):
-                raise TypeError(f"The 'required_envs' attribute type <{type(required_envs).__name__}> is invalid, must be a <list>!")
-        except TypeError as err:
-            logger.exception(err)
-            exit(2)
+    def required_envs(self, required_envs: List[str]):
+        if not isinstance(required_envs, list):
+            raise TypeError(
+                f"The 'required_envs' attribute type {type(required_envs)} is invalid, must be a <list>!"
+            )
+
+        if not all(isinstance(_val, str) for _val in required_envs):
+            raise ValueError(
+                f"The 'required_envs' attribute value {required_envs} is invalid, must be a list of <str>!"
+            )
 
         self.__required_envs = required_envs
-    ## required_envs ##
 
+    ## required_envs ##
 
-    ## valid_schema ##
+    ## pre_load_hook ##
     @property
-    def valid_schema(self):
+    def pre_load_hook(self) -> Union[Callable, None]:
         try:
-            return self.__valid_schema
+            return self.__pre_load
         except AttributeError:
-            return None
+            return ConfigLoader._PRE_LOAD_HOOK
 
-    @valid_schema.setter
-    def valid_schema(self, valid_schema):
-        try:
-            if not isinstance(valid_schema, dict):
-                raise TypeError(f"The 'valid_schema' attribute type <{type(valid_schema).__name__}> is invalid, must be a <dict>!")
-        except TypeError as err:
-            logger.exception(err)
-            exit(2)
+    @pre_load_hook.setter
+    def pre_load_hook(self, pre_load_hook: Callable):
+        if not callable(pre_load_hook):
+            raise TypeError(
+                f"'pre_load_hook' argument type {type(pre_load_hook)} is invalid, should be callable <function>!"
+            )
+
+        self.__pre_load = pre_load_hook
 
-        self.__valid_schema = valid_schema
-    ## valid_schema ##
+    ## pre_load_hook ##
     ### ATTRIBUTES ###
```

### Comparing `onion_config-1.0.1/setup.py` & `onion_config-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 from distutils.util import convert_path
 
 
-_package_name = 'onion_config'
+_package_name = "onion_config"
 
 _namespace_dict = {}
-_version_path = convert_path(f'{_package_name}/__version__.py')
+_version_path = convert_path(f"{_package_name}/__version__.py")
 with open(_version_path) as _version_file:
     exec(_version_file.read(), _namespace_dict)
-_package_version = _namespace_dict['__version__']
+_package_version = _namespace_dict["__version__"]
 
 setup(
-    name = _package_name,
-    packages = [_package_name],
-    version = f"{_package_version}",
-    license='MIT',
-    description = 'Python-box based custom config package (onion_config) for python projects.',
-    long_description = open('README.md', 'r').read(),
-    long_description_content_type = 'text/markdown',
-    author = 'Batkhuu Byambajav',
-    author_email = 'batkhuu10@gmail.com',
-    url = 'https://github.com/bybatkhuu/python_config',
-    download_url = f'https://github.com/bybatkhuu/python_config/archive/v{_package_version}.tar.gz',
-    keywords = [_package_name, 'config', 'configs', 'python-box', 'custom-config'],
-    install_requires = [
-        'python-dotenv>=0.20.0',
-        'Cerberus>=1.3.4',
-        'PyYAML>=6.0',
-        'python-box[PyYAML]>=6.0.2'
+    name=_package_name,
+    packages=[_package_name],
+    version=f"{_package_version}",
+    license="MIT",
+    description="onion_config is a Python package that allows for easy configuration management. It allows for loading and validating configuration data from environment variables and config files in JSON and YAML formats.",
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
+    author="Batkhuu Byambajav",
+    author_email="batkhuu10@gmail.com",
+    url="https://github.com/bybatkhuu/mod.python-config",
+    download_url=f"https://github.com/bybatkhuu/mod.python-config/archive/v{_package_version}.tar.gz",
+    keywords=[
+        _package_name,
+        "config",
+        "configs",
+        "python-dotenv",
+        "python-box",
+        "pydantic",
+        "pydantic-config",
+        "custom-config",
+    ],
+    python_requires=">=3.7",
+    install_requires=[
+        "python-dotenv>=1.0.0",
+        "PyYAML>=6.0",
+        "email-validator==1.3.1",
+        "python-box>=7.0.1",
+        "pydantic==1.10.9",
+    ],
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    classifiers = [
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
-    ]
 )
```

