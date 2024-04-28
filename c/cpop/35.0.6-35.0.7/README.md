# Comparing `tmp/cpop-35.0.6.tar.gz` & `tmp/cpop-35.0.7.tar.gz`

## Comparing `cpop-35.0.6.tar` & `cpop-35.0.7.tar`

### file list

```diff
@@ -1,176 +1,179 @@
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.6/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/data.pyx
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/exc.pyx
--rw-r--r--   0        0        0    27276 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/hub.pyx
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/ref.pyx
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.6/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/config.yaml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/log/basic.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/log/init.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0     9610 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/mods/task.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cpop-35.0.6/src/pop/mods/test.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_ref.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_sub.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/func/test_task.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/vtrue.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/unit/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.6/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.6/.gitignore
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.0.6/README.rst
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.0.6/pyproject.toml
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.0.6/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-35.0.7/.coveragerc
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.7/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/data.pyx
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    28261 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/hub.pyx
+-rw-r--r--   0        0        0    10445 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.7/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/config.yaml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/basic.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/init.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9610 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/task.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cpop-35.0.7/src/pop/mods/test.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_ref.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_relative.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_sub.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/func/test_task.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/bad.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/dunder.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/unit/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.7/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.7/.gitignore
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.0.7/README.rst
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.0.7/PKG-INFO
```

### Comparing `cpop-35.0.6/.pre-commit-config.yaml` & `cpop-35.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/Makefile` & `cpop-35.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/make.bat` & `cpop-35.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/outline.rst` & `cpop-35.0.7/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/conf.py` & `cpop-35.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/index.rst` & `cpop-35.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/app_merging.rst` & `cpop-35.0.7/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/conf.rst` & `cpop-35.0.7/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/conf_integrate.rst` & `cpop-35.0.7/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/contracts.rst` & `cpop-35.0.7/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/dyne_name.rst` & `cpop-35.0.7/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/func_alias.rst` & `cpop-35.0.7/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/glossary.rst` & `cpop-35.0.7/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/hub_overview.rst` & `cpop-35.0.7/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-35.0.7/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/learning.rst` & `cpop-35.0.7/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/pop.rst` & `cpop-35.0.7/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/pre_contract_returns.rst` & `cpop-35.0.7/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/story.rst` & `cpop-35.0.7/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/sub_patterns.rst` & `cpop-35.0.7/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/subs_overview.rst` & `cpop-35.0.7/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/topics/virtual.rst` & `cpop-35.0.7/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/docs/source/tutorial/quickstart.rst` & `cpop-35.0.7/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/cpop/contract.pyx` & `cpop-35.0.7/src/cpop/contract.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -99,40 +99,55 @@
 cdef class Contracted:
     """
     This class wraps functions that have a contract associated with them
     and executes the contract routines
     """
     cdef:
         public bint _has_contracts
-        public bint implicit_hub
+        cdef public bint implicit_hub
         public dict[str, list[object]] contract_functions
         public object hub
         public object func
         public object signature
-        public str __name__
-        public str ref
+        cdef public str __name__
+        cdef public str ref
         list _sig_errors
         list contracts
         object __wrapped__
+        object parent
 
-    def __init__(self, hub, contracts: list, func: object, ref: str, name: str, implicit_hub: bool = True):
+    def __init__(
+                self,
+                hub,
+                contracts: list,
+                func: object,
+                ref: str,
+                name: str,
+                parent: object,
+                implicit_hub: bool = True
+            ):
         self.__name__ = name
         self.__wrapped__ = func
         self._sig_errors = []
         self.contracts = contracts or []
+        self.parent = parent
         self.func = func
         self.hub = hub
         self.implicit_hub = implicit_hub
-        self.ref = ref
+        self.ref = f"{ref}.{name}"
         # Manually define the function signature if needed
         self.signature = inspect.signature(self.func)
 
         self._load_contracts()
 
     @property
+    def __(self):
+        return self.parent
+
+    @property
     def __signature__(self):
         return self.signature
 
     @property
     def __dict__(self):
         return self.func.__dict__
 
@@ -211,15 +226,15 @@
         self.ref = state["ref"]
         self.__name__ = state["name"]
         self.func = self.hub[self.ref][self.__name__].func
         self.implicit_hub = state["implicit_hub"]
         self.contracts = state["contracts"]
 
     def __repr__(self):
-        return f"<{self.__class__.__name__} {self.ref}.{self.__name__}>"
+        return f"<{self.__class__.__name__} {self.ref}>"
 
 
 class ContractedAsyncGen(Contracted):
     async def __call__(self, *args, **kwargs):
         async with CallStack(self):
             if self.implicit_hub:
                 args = (self.hub,) + args
@@ -261,35 +276,37 @@
         self.contract = contract
 
     async def __aenter__(self):
         # Get the caller's frame
         frame = sys._getframe(1)
         stack_summary = traceback.StackSummary.extract(traceback.walk_stack(frame))
         # Push the ref and the stack summary onto the call stack
-        self.contract.hub._call_stack_push(f"{self.contract.ref}.{self.contract.__name__}", stack_summary)
+        self.contract.hub._call_stack_push(self.contract.ref, stack_summary)
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         # Remove the entry from the call stack
         self.contract.hub._call_stack_pop()
 
 
 def create_contracted(
     hub,
     contracts: list["cpop.loader.LoadedMod"],
     func,
     ref: str,
     name: str,
+    parent: object,
     implicit_hub: bool = True,
 ) -> Contracted:
     """
     Dynamically create the correct Contracted type
     :param hub: The redistributed pop central hub
     :param contracts: Contracts functions to add to the sub
     :param func: The contracted function to call
     :param ref: The reference to the function on the hub
     :param name: The name of the module to get from the loader
+    :param parent: The object on the namespace above this contract
     :param implicit_hub: True if a hub should be implicitly injected into the "call" method
     """
     if inspect.isasyncgenfunction(func):
         return ContractedAsyncGen(hub, contracts, func, ref, name, implicit_hub)
     else:
-        return Contracted(hub, contracts, func, ref, name, implicit_hub)
+        return Contracted(hub, contracts, func, ref, name, parent, implicit_hub)
```

### Comparing `cpop-35.0.6/src/cpop/data.pyx` & `cpop-35.0.7/src/cpop/data.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,30 @@
         self[key] = value
 
 
 cdef class MultidictCache:
     cdef dict[str, object] _cache
     cdef list[dict[str, object]] _base_dicts
     cdef dict[str, list[str]] _split_cache
+    cdef object _root
 
-    def __init__(self, base_dicts=None):
+    def __init__(self, base_dicts=None, parent: object = None):
         if base_dicts is None:
             base_dicts = []
         self._base_dicts = base_dicts
         self._cache = dict[str, object]()
         self._split_cache = dict[str, list[str]]()
+        self._root = parent or self
+
+    @property
+    def __(self):
+        """
+        Let any instance of MultidictCache access its parent in this way
+        """
+        return self._root
 
     cpdef _clear(self):
         self._cache.clear()
         self._split_cache.clear()
 
     def __getitem__(self, key: str):
         if key in self._cache:
```

### Comparing `cpop-35.0.6/src/cpop/dirs.pyx` & `cpop-35.0.7/src/cpop/dirs.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/cpop/exc.pyx` & `cpop-35.0.7/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/cpop/hub.pyx` & `cpop-35.0.7/src/cpop/hub.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
 SHUTDOWN_SIGNAL = object()
 
 
 class PopMeta(cpop.data.MultidictCache):
     _subs = None
 
-    def __init__(self, data: list[dict[str, any]]):
+    def __init__(self, data: list[dict[str, any]], parent: object):
         attrs = {}
         data.append(attrs)
-        super().__init__(data)
+        super().__init__(data, parent = parent)
         object.__setattr__(self, "_attrs", attrs)
 
     def __setitem__(self, key: str, value):
         # Recurse the dotted reference and set the value on the last part of the reference
         if "." in key:
             parts = key.split(".")
             finder = self
@@ -87,15 +87,15 @@
             ):
         self.__init_kwargs = {
             k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
         }
         subs = {}
         sub_alias = {}
         imports = {}
-        PopMeta.__init__(self, [subs, sub_alias, imports])
+        PopMeta.__init__(self, [subs, sub_alias, imports], parent=self)
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._dynamic = None
         self._dscan = False
         # Set up the conf OPT structure so it is always available
         self._opt = None
@@ -158,14 +158,28 @@
             self._traceback(exc_type, exc_value, tb)
         await self._tasks.put(SHUTDOWN_SIGNAL)
 
     @property
     def OPT(self):
         return self._opt
 
+    @property
+    def _(self):
+        """
+        Return the parent of the last function on the call stack
+        """
+        stack = self._call_stack.get()
+        if stack:
+            last_ref = stack[len(stack) - 1][0]
+            last_mod = last_ref.rsplit(".", maxsplit=1)[0]
+            return cpop.ref.last(self, last_mod)
+
+        # If nothing else worked return an instance of the hub
+        return self
+
     async def _load_all(self):
         for base, imp in self._dynamic.imports__.items():
             self._subs["lib"]._imports[base] = imp
 
         # Load all dynamic subs onto the hub
         for dyne in self._dynamic.dyne:
             if dyne in self._subs:
@@ -346,14 +360,15 @@
         stop_on_failures: bool = False,
         init: bool = True,
         is_contract: bool = False,
         sub_virtual: bool = True,
         recursive_contracts_static: list[str] = None,
         default_recursive_contracts: list[str] = None,
         lookup_paths: list[dict] = None,
+        parent: object = None,
     ):
         """
         :param hub: The redistributed pop central hub
         :param subname: The name that the sub is going to take on the hub
             if nothing else is passed, it is used as the pypath
         :param pypath: One or many python paths which will be imported
         :param static: Directories that can be explicitly passed
@@ -389,27 +404,30 @@
         loaded = {}
 
         # tracks what has been setattr-ed on this sub for performance; if something needs to be
         # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
         if lookup_paths is None:
             lookup_paths = []
 
-        super().__init__([loaded, imports, subs, sub_alias] + lookup_paths)
+        _root = root or hub
+        self._parent = parent or _root
+
+        super().__init__([loaded, imports, subs, sub_alias] + lookup_paths, parent=self._parent)
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._loaded = loaded
         self._reload_mods = {}
         self._alias = []
         self._loaded_all = False
         self._load_errors = {}
         self._vmap = {}
         self._hub = hub
-        self._root = root or hub
-        self._subname = subname
+        self._root = _root
+        self.__name__ = self._subname = subname
         self._pypath = ex_path(pypath)
         self._static = ex_path(static)
         self._contracts_pypath = ex_path(contracts_pypath)
         self._contracts_static = ex_path(contracts_static)
         self._recursive_contracts_static = ex_path(recursive_contracts_static)
         self._default_recursive_contracts = default_recursive_contracts or []
         self._default_contracts = default_contracts or ()
@@ -450,14 +468,15 @@
             await cpop.dirs.inline_dirs(self._dirs, "recursive_contracts")
         )
 
         self._contract_subs = []
         for i in range(len(self._contract_dirs)):
             sub = await AsyncSub(
                 hub=self._hub,
+                parent=self,
                 subname=f"{self._subname}._contract_subs[{i}]",
                 static=[self._contract_dirs[i]],
                 is_contract=True,
             )
             await sub._load_all()
             self._contract_subs.append(sub)
 
@@ -469,14 +488,15 @@
             # child Subs look at the parent's _recursive_contract_dirs, so we can't modify it
             filtered_recursive_contract_dirs = sorted(
                 set(self._recursive_contract_dirs) - set(self._contract_dirs)
             )
             for i in range(len(filtered_recursive_contract_dirs)):
                 sub = await AsyncSub(
                     hub=self._hub,
+                    parent=self,
                     subname=f"{self._subname}._recursive_contract_subs[{i}]",
                     static=[filtered_recursive_contract_dirs[i]],
                     is_contract=True,
                 )
                 await sub._load_all()
                 self._recursive_contract_subs.append(sub)
         else:
@@ -681,20 +701,20 @@
         :param mod: A python module containing data
         :param iface: A scanned directory type
         :param bname: The base name of the python path of a module
         """
         if not self._sub_virtual:
             return
         else:
-            vret = await cpop.loader.load_sub_virtual(self._hub, mod, bname)
+            vret = await cpop.loader.load_sub_virtual(self._hub, mod, bname, self._ref)
             if self._process_vret(vret):
                 self._sub_virtual = False
                 return
 
-        vret = await cpop.loader.load_virtual(self._hub, mod, bname)
+        vret = await cpop.loader.load_virtual(self._hub, mod, bname, self._ref)
 
         if self._process_vret(vret):
             return
 
         contracts = []
         for contract_sub in self._contract_subs:
             contracts.extend(
@@ -737,14 +757,26 @@
         for iface in self._scan:
             for bname in self._scan[iface]:
                 if self._scan[iface][bname].get("loaded"):
                     continue
                 await self._load_item(iface, bname)
         self._loaded_all = True
 
+    @property
+    def _ref(self) -> str:
+        """
+        Return a full path on the hub to this sub
+        """
+        ref = self._subname
+        root = self._parent
+        while hasattr(root, "_subname"):
+            ref = f"{root._subname}.{ref}"
+            root = root._parent
+        return ref
+
 
 cdef class AsyncInitWrapper:
     cdef object cls
 
     def __init__(self, cls):
         self.cls = cls
```

### Comparing `cpop-35.0.6/src/cpop/loader.pyx` & `cpop-35.0.7/src/cpop/loader.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 
 
 async def _load_virtual(
     hub,
     mod: "LoadedMod" or LoadError,
     bname: str,
     vtype: str,
+    ref: str,
 ) -> dict[str, Any]:
     """
     Run the virtual function to name the module and check for all loader
     errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
@@ -91,15 +92,23 @@
     if not hasattr(mod, vtype):
         # No __virtual__ processing is required.
         # Return the mod's name as the defined __virtualname__ if defined,
         # else, the base_name
         return {"name": name}
 
     try:
-        vret = await getattr(mod, vtype)(hub)
+        virtual_func = cpop.contract.Contracted(
+            hub,
+            contracts=[],
+            func=getattr(mod, vtype),
+            ref=f"{ref}.{name}",
+            parent=mod,
+            name="__virtual__",
+        )
+        vret = await virtual_func()
     except Exception as e:
         vret = False, str(e)
 
     verror = vret
     if isinstance(vret, tuple):
         if len(vret) > 1:
             verror = vret[1]
@@ -115,39 +124,39 @@
         err = LoadError(f"Module {bname} returned virtual FALSE", verror=verror)
         # Return the load error with name as the base_name because another
         # module is still allowed to load under the same __virtualname__
         # but also return the vname information
         return {"name": base_name, "vname": name, "error": err}
 
 
-async def load_virtual(hub, mod: "LoadedMod" or LoadError, bname: str) -> dict[str, Any]:
+async def load_virtual(hub, mod: "LoadedMod" or LoadError, bname: str, ref:str) -> dict[str, Any]:
     """
     Run the __virtual__ function to name the module and check for all loader errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
     :param bname: The base name of the mod's path
     """
-    return await _load_virtual(hub, mod, bname, "__virtual__")
+    return await _load_virtual(hub, mod, bname, "__virtual__", ref)
 
 
 async def load_sub_virtual(
-    hub, mod: "LoadedMod" or LoadError, bname: str
+    hub, mod: "LoadedMod" or LoadError, bname: str, ref:str
 ) -> dict[str, Any]:
     """
     Run the __sub_virtual__ function to name the module and check for all loader errors
     :param hub: The redistributed pop central hub
     :param virtual: Toggle whether or not to process __virtual__ functions
     :param mod: A loader module or a LoadError if the module didn't load
     :param bname: The base name of the mod's path
     """
     _, name = _base_name(bname, mod)
     if name != "init":
         return {"name": name}
-    return await _load_virtual(hub, mod, bname, "__sub_virtual__")
+    return await _load_virtual(hub, mod, bname, "__sub_virtual__", ref)
 
 
 async def mod_init(sub, mod: "LoadedMod", mod_name: str):
     """
     Process module's __init__ function if defined
     :param sub: The pop object that contains the loaded module data
     :param mod: A loader modul
@@ -155,14 +164,15 @@
     """
     if "__init__" in dir(mod):
         init = cpop.contract.Contracted(
             sub._hub,
             contracts=[],
             func=mod.__init__,
             ref=f"{sub._subname}.{mod_name}",
+            parent=mod,
             name="__init__",
         )
         await init()
 
 
 def sub_alias(this_sub, mod: "LoadedMod", mod_name: str):
     """
@@ -178,29 +188,23 @@
             this_sub._alias = alias
 
 
 async def prep_loaded_mod(
     this_sub,
     mod: "LoadedMod",
     mod_name: str,
-    contracts: "List[cpop.contract.Wrapper]",
-    recursive_contracts: "List[cpop.contract.Wrapper]",
+    contracts: "list[cpop.contract.Wrapper]",
+    recursive_contracts: "list[cpop.contract.Wrapper]",
 ) -> "LoadedMod":
     ordered_contracts = contracts + recursive_contracts
 
-    lmod = this_sub._loaded.get(mod_name, LoadedMod(mod_name))
+    lmod = this_sub._loaded.get(mod_name, LoadedMod(mod_name, parent=this_sub))
 
     # getattr(hub, ref) should resolve to this module
-    ref = f"{this_sub._subname}.{mod_name}"
-
-    # Get the full path to this module on the hub
-    root = this_sub._root
-    while hasattr(root, "_subname"):
-        ref = f"{root._subname}.{ref}"
-        root = root._root
+    ref = f"{this_sub._ref}.{mod_name}"
 
     sub_alias(this_sub, mod, mod_name)
     func_alias_dict: dict[str, Union[str, Callable, cpop.contract.Contracted]] = {}
 
     __func_alias__: Union[Callable, dict[str, Union[str, Callable]]] = getattr(mod, "__func_alias__", {})
     if asyncio.iscoroutinefunction(__func_alias__):
         func_alias_dict.update(await __func_alias__(this_sub._hub))
@@ -220,15 +224,15 @@
             setattr(lmod, name, func)
             continue
 
         if attr.startswith(tuple(this_sub._omit_start)) or attr.endswith(tuple(this_sub._omit_end)):
             continue
 
         if inspect.isfunction(func) or inspect.isbuiltin(func) or type(func).__name__ == "cython_function_or_method":
-            obj = cpop.contract.create_contracted(this_sub._hub, ordered_contracts, func, ref, name)
+            obj = cpop.contract.create_contracted(this_sub._hub, ordered_contracts, func, ref, name, parent=lmod)
             if not this_sub._omit_func and (not this_sub._pypath or func.__module__.startswith(mod.__name__)):
                 lmod._funcs[name] = obj
         elif not this_sub._omit_class and inspect.isclass(func) and func.__module__.startswith(mod.__name__):
             lmod._classes[name] = func
 
     for attr, func_alias in func_alias_dict.items():
         if isinstance(func_alias, cpop.contract.Contracted):
@@ -236,14 +240,15 @@
         elif isinstance(func_alias, Callable):
             obj = cpop.contract.create_contracted(
                 this_sub._hub,
                 ordered_contracts,
                 func_alias,
                 ref,
                 attr,
+                parent=lmod,
                 implicit_hub=False
             )
         else:
             continue
         lmod._funcs[attr] = obj
 
     return lmod
@@ -252,26 +257,28 @@
 class LoadedMod(types.ModuleType):
     """
     The LoadedMod class allows for the module loaded onto the sub to return
     custom sequencing, for instance it can be iterated over to return all
     functions
     """
 
-    def __init__(self, name: str):
+    def __init__(self, name: str, parent: cpop.hub.Sub):
         super().__init__(name)
         cdef dict vars = {}
         cdef dict funcs = {}
         cdef dict classes = {}
-        self._attrs = cpop.data.MultidictCache([funcs, classes, vars])
+        self._attrs = cpop.data.MultidictCache([funcs, classes, vars], parent=parent)
         self._vars = vars
         self._funcs = funcs
         self._classes = classes
 
     def __getattr__(self, item: str):
-        if item.startswith("_"):
+        if item == "__":
+            return self._attrs.__
+        elif item.startswith("_"):
             return self.__getattribute__(item)
         try:
             return self._attrs[item]
         except KeyError as e:
             raise AttributeError(e)
 
     def __getitem__(self, item: str):
```

### Comparing `cpop-35.0.6/src/cpop/ref.pyx` & `cpop-35.0.7/src/cpop/ref.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/cpop/scanner.pyx` & `cpop-35.0.7/src/cpop/scanner.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/cpop/verify.pyx` & `cpop-35.0.7/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/config.yaml` & `cpop-35.0.7/src/pop/config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/log/basic.py` & `cpop-35.0.7/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/log/init.py` & `cpop-35.0.7/src/pop/log/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/log/timed_rolling.py` & `cpop-35.0.7/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/mods/config.py` & `cpop-35.0.7/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/mods/contract.py` & `cpop-35.0.7/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/mods/sub.py` & `cpop-35.0.7/src/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/mods/task.py` & `cpop-35.0.7/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/src/pop/mods/test.py` & `cpop-35.0.7/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/conftest.py` & `cpop-35.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/contracts/ctx.py` & `cpop-35.0.7/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/contracts/many.py` & `cpop-35.0.7/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/contracts/test.py` & `cpop-35.0.7/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_basic.py` & `cpop-35.0.7/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_config.py` & `cpop-35.0.7/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_contract_ctx.py` & `cpop-35.0.7/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_fail.py` & `cpop-35.0.7/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_log.py` & `cpop-35.0.7/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_no_raise_on_pre_failure.py` & `cpop-35.0.7/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_raise_on_pre_failure.py` & `cpop-35.0.7/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_ref.py` & `cpop-35.0.7/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/func/test_serial.py` & `cpop-35.0.7/tests/func/test_serial.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-35.0.7/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-35.0.7/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/mods/proc.py` & `cpop-35.0.7/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/mods/test.py` & `cpop-35.0.7/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/regression/contract_masking/test_contract_masking.py` & `cpop-35.0.7/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-35.0.7/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/tpath/cn/contract/test.py` & `cpop-35.0.7/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/tests/unit/test_contract.py` & `cpop-35.0.7/tests/unit/test_contract.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from cpop.contract import Contracted
 
 
 async def test_contracted_shortcut(hub):
     async def f(hub):
         pass
 
-    c = Contracted(hub=hub, contracts=[], func=f, ref="", name="")
+    c = Contracted(hub=hub, contracts=[], func=f, ref="", name="", parent=None)
     c.contract_functions["pre"] = [
         None
     ]  # add some garbage so we raise if we try to evaluate contracts
 
     await c()
 
 
 async def test_contracted_inspect():
     def f(hub, p1, p2=None):
         pass
 
-    c = Contracted(None, [], f, "", "")
+    c = Contracted(None, [], f, "", "", None)
 
     assert str(inspect.signature(c)) == str(inspect.signature(f))
     assert str(inspect.signature(c)) == "(hub, p1, p2=None)"
```

### Comparing `cpop-35.0.6/tests/unit/test_sigs.py` & `cpop-35.0.7/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/.gitignore` & `cpop-35.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/README.rst` & `cpop-35.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.6/pyproject.toml` & `cpop-35.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython", "hatch-compile-yaml>=18.0.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "35.0.6"
+version = "35.0.7"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-35.0.6/PKG-INFO` & `cpop-35.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 35.0.6
+Version: 35.0.7
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

