
学习使用RQAlpha

https://github.com/ricequant/rqalpha

安装python 3.6,配置python连接到3.6:
alias python="python3.6"

sudo pip3 install -U pip setuptools

安装 cython 库:

sudo pip3 install cython

安装 RQAlpha

sudo pip3 install rqalpha

报错:
No local packages or working download links found for setuptools-scm>1.5.4
    Traceback (most recent call last):
      File "<string>", line 1, in <module>
      File "/private/tmp/pip-build-wglxxm2v/bcolz/setup.py", line 228, in <module>
        cmdclass=LazyCommandClass(),
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/distutils/core.py", line 108, in setup
        _setup_distribution = dist = klass(attrs)
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/setuptools/dist.py", line 317, in __init__
        self.fetch_build_eggs(attrs['setup_requires'])
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/setuptools/dist.py", line 372, in fetch_build_eggs
        replace_conflicting=True,
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/pkg_resources/__init__.py", line 851, in resolve
        dist = best[req.key] = env.best_match(req, ws, installer)
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/pkg_resources/__init__.py", line 1123, in best_match
        return self.obtain(req, installer)
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/pkg_resources/__init__.py", line 1135, in obtain
        return installer(requirement)
      File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/setuptools/dist.py", line 440, in fetch_build_egg
        return cmd.easy_install(req)
File "/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages/setuptools/command/easy_install.py", line 668, in easy_install
        raise DistutilsError(msg)
    distutils.errors.DistutilsError: Could not find suitable distribution for Requirement.parse('setuptools-scm>1.5.4')
    SSE2 detected

    ----------------------------------------
Command "python setup.py egg_info" failed with error code 1 in /private/tmp/pip-build-wglxxm2v/bcolz/

sudo easy_install setuptools_scm-1.15.0-py3.6.egg

重新执行:sudo pip3 install rqalpha