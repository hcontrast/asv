0.2 (unreleased)
----------------

New Features
^^^^^^^^^^^^

- Automatic detection and listing of performance regressions. (#236)
- Support for Windows. (#282)
- New ``setup_cache`` method. (#277)
- Exclude/include rules in configuration matrix. (#329)

API Changes
^^^^^^^^^^^

- Mirrors are no longer created for local repositories. (#314)
- The parent directory of the benchmark suite is no longer inserted
  into ``sys.path``. (#307)
- In asv.conf.json matrix, ``null`` previously meant (undocumented)
  the latest version. Now it means that the package is to not be
  installed. (#329)
- Previously, the ``setup`` and ``teardown`` methods were run only once
  even when the benchmark method was run multiple times, for example due
  to ``repeat > 1`` being present in timing benchmarks. This is now
  changed so that also they are run multiple times. (#316)

Bug Fixes
^^^^^^^^^

- Output will display on non-Unicode consoles. (#313, #318)
- Various bugfixes and minor improvements. (#276, #284, #289, #291,
  #295, #298, #300, #302, #304, #306, #307, #315, #321, #325)

Other Changes and Additions
^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.1.1 (2015-05-05)
------------------

First full release.

0.1rc3 (2015-05-01)
-------------------

Bug Fixes
^^^^^^^^^
Include pip_requirements.txt.

Display version correctly in docs.

0.1rc2 (2015-05-01)
-------------------

0.1rc1 (2015-05-01)
-------------------
