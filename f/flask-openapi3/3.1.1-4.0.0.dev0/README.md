# Comparing `tmp/flask_openapi3-3.1.1.tar.gz` & `tmp/flask_openapi3-4.0.0.dev0.tar.gz`

## Comparing `flask_openapi3-3.1.1.tar` & `flask_openapi3-4.0.0.dev0.tar`

### file list

```diff
@@ -1,120 +1,111 @@
--rw-r--r--   0        0        0    11199 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/api_blueprint_demo.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/api_view_demo.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/async_demo.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/custom_ui_templates_demo.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/enum_demo.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/header_demo.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/image_demo.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/init_oauth_demo.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/just_flask.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/nested_apiblueprint_demo.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/openapi_extensions.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/openapi_extra.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/orjson_demo.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/pydantic_custom_root_types.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/raw_request_demo.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/response_demo.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/rest_demo.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/servers_demo.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/simple_demo.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/examples/upload_file_demo.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/__version__.py
--rw-r--r--   0        0        0     8203 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/blueprint.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/commands.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/markdown.py
--rw-r--r--   0        0        0    18986 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/openapi.py
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/request.py
--rw-r--r--   0        0        0    17791 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/scaffold.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/types.py
--rw-r--r--   0        0        0    21294 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/utils.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/view.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/callback.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/components.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/contact.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/data_type.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/discriminator.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/encoding.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/external_documentation.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/file.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/header.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/info.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/license.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/link.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/media_type.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/oauth_flow.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/oauth_flows.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/operation.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/parameter.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/parameter_in_type.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/path_item.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/paths.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/reference.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/request_body.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/response.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/responses.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/schema.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/security_requirement.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/security_scheme.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/security_scheme_in_type.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/server.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/server_variable.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/style_values.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/tag.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/validation_error.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/models/xml.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/__init__.py
--rw-r--r--   0        0        0   152042 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/css/swagger-ui.css
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/images/swagger.svg
--rw-r--r--   0        0        0   662202 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0        0        0   870152 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0        0        0  1415333 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0        0        0   230777 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/build.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/doc.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/flake8.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/mypy.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/requirements/test.txt
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_api_blueprint.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_api_view.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_api_view_args.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_async.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_custom_ui_templates_demo.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_default_query.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_empty_body.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_enum.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_fixed_externaldocs_support.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_form.py
--rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_model_config.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_multi_decorator.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_nested_apiblueprint.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_number_constraints.py
--rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_openapi.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_openapi_extensions.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_options_in_viewfunc.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_pydantic_calculated_fields.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_pydantic_custom_root_types.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_request.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_response.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_restapi.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_restapi_with_doc_prefix.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_security.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_str_body.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_summary.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_swagger_config.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_tags.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_trail_slash.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/tests/test_validation_error.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/LICENSE.rst
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/README.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 flask_openapi3-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/api_blueprint_demo.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/api_view_demo.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/async_demo.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/custom_ui_templates_demo.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/enum_demo.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/header_demo.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/image_demo.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/init_oauth_demo.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/just_flask.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/openapi_extensions.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/openapi_extra.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/orjson_demo.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/pydantic_custom_root_types.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/raw_request_demo.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/response_demo.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/rest_demo.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/servers_demo.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/simple_demo.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/examples/upload_file_demo.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/__version__.py
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/blueprint.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/commands.py
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/markdown.py
+-rw-r--r--   0        0        0    18389 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/openapi.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/plugins.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/request.py
+-rw-r--r--   0        0        0    18229 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/scaffold.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/templates.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/types.py
+-rw-r--r--   0        0        0    21890 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/utils.py
+-rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/view.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/callback.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/components.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/contact.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/data_type.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/discriminator.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/encoding.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/example.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/external_documentation.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/file.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/header.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/info.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/license.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/link.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/media_type.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/oauth_flow.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/oauth_flows.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/operation.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/parameter.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/parameter_in_type.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/path_item.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/paths.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/reference.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/request_body.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/response.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/responses.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/schema.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/security_requirement.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/security_scheme.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/security_scheme_in_type.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/server.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/server_variable.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/style_values.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/tag.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/validation_error.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/flask_openapi3/models/xml.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/requirements/build.txt
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/requirements/doc.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/requirements/flake8.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/requirements/mypy.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/requirements/test.txt
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_api_blueprint.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_api_view.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_api_view_args.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_async.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_default_query.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_empty_body.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_enum.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_fixed_externaldocs_support.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_form.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_model_config.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_multi_decorator.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_nested_apiblueprint.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_number_constraints.py
+-rw-r--r--   0        0        0    16323 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_openapi.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_openapi_extensions.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_options_in_viewfunc.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_pydantic_calculated_fields.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_pydantic_custom_root_types.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_request.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_response.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_restapi.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_restapi_with_doc_prefix.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_security.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_str_body.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_summary.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_swagger_config.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_tags.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_trail_slash.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_utils.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/tests/test_validation_error.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/LICENSE.rst
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/README.md
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 flask_openapi3-4.0.0.dev0/PKG-INFO
```

### Comparing `flask_openapi3-3.1.1/CHANGELOG.md` & `flask_openapi3-4.0.0.dev0/CHANGELOG.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,282 +1,282 @@
-## v3.1.1 2024-04-21
-
-- Wrong types of exclusiveMinimum & exclusiveMaximum fields in Schema class by @Lavertis in #149
-
-## v3.1.0 2024-03-24
-
-- Add the swagger_config parameter to configure the swagger ui by @luolingchun in #146
-- Use full links in Swagger and RapiDoc
-- Upgrade Redoc to 2.1.3
-- Upgrade Swagger to 5.12.0
-
-**DeprecationWarning**
-
-- The doc_expansion parameter is deprecated; use swagger_config instead.
-
-## v3.0.2 2024-01-28
-
-- Fix missing Pydantic Calculated Fields (#141). Thanks, @thebmw.
-
-## v3.0.1 2023-11-26
-
-- Fix the same operationId in APIBlueprint (#133). Thanks, @fluffybrain3.
-- Make body required false (#130). Thanks, @styper.
-- The default value defined in the form is invalid (#129). Thanks, @seekplum.
-
-## v3.0.0 2023-10-22
-
-- Upgrade pydantic to v2.
-- Remove deprecated code.
-- Drop support for Python 3.7.
-- support for raw requests (#109).
-- Upgrade Swagger UI v5.9.0.
-- Upgrade Redoc v2.1.2
-- Update RapiDoc 9.3.4.
-- [#105](https://github.com/luolingchun/flask-openapi3/pull/105) Supports valid properties only. Thanks, @ota42y.
-- [#106](https://github.com/luolingchun/flask-openapi3/pull/106) Bugfix for parameter object. Thanks, @ota42y.
-- [#107](https://github.com/luolingchun/flask-openapi3/pull/107) Bugfix for generics class. Thanks, @ota42y.
-- [#114](https://github.com/luolingchun/flask-openapi3/pull/114) Support Flask 3.0.
-- [#118](https://github.com/luolingchun/flask-openapi3/discussions/118) Fix missed components schemas in ValidationErrorModel. Thanks, @SeFeX.
-- [#122](https://github.com/luolingchun/flask-openapi3/issues/122) Skip 422 response non parameters. Thanks, @Danielsn1.
-
-
-## v3.0.0rc2 2023-10-03
-
-- [#105](https://github.com/luolingchun/flask-openapi3/pull/105) Supports valid properties only. Thanks, @ota42y.
-- [#106](https://github.com/luolingchun/flask-openapi3/pull/106) Bugfix for parameter object. Thanks, @ota42y.
-- [#107](https://github.com/luolingchun/flask-openapi3/pull/107) Bugfix for generics class. Thanks, @ota42y.
-- [#114](https://github.com/luolingchun/flask-openapi3/pull/114) Support Flask 3.0.
-
-## v3.0.0rc1 2023-09-03
-
-- Upgrade pydantic to v2
-- Remove deprecated code
-- Drop support for Python 3.7
-
-## v2.5.5 2023-11-26
-
-- Fix the same operationId in APIBlueprint (#133). Thanks, @fluffybrain3.
-- Make body required false (#130). Thanks, @styper.
-- The default value defined in the form is invalid (#129). Thanks, @seekplum.
-
-## v2.5.4 2023-10-22
-
-- [#118](https://github.com/luolingchun/flask-openapi3/discussions/118) Fix missed components schemas in ValidationErrorModel. Thanks, @SeFeX.
-- [#122](https://github.com/luolingchun/flask-openapi3/issues/122) Skip 422 response non parameters. Thanks, @Danielsn1.
-
-## v2.5.3 2023-10-03
-
-- [#105](https://github.com/luolingchun/flask-openapi3/pull/105) Supports valid properties only. Thanks, @ota42y.
-- [#106](https://github.com/luolingchun/flask-openapi3/pull/106) Bugfix for parameter object. Thanks, @ota42y.
-- [#107](https://github.com/luolingchun/flask-openapi3/pull/107) Bugfix for generics class. Thanks, @ota42y.
-
-## v2.5.2 2023-08-13
-
-- [#97](https://github.com/luolingchun/flask-openapi3/issues/97) Fix response miss description. Thanks, @tekrei.
-
-## v2.5.1 2023-08-07
-
-- [#95](https://github.com/luolingchun/flask-openapi3/pull/95) Added ability to deserialize complex form parameter objects. Thanks, @BlackGad.
-
-## v2.5.0 2023-08-02
-
-- [#79](https://github.com/luolingchun/flask-openapi3/discussions/79) Support `by_alias` in Model Config. Thanks, @candleindark.
-- [#82](https://github.com/luolingchun/flask-openapi3/issues/82) Fix parameter in url_prefix. Thanks, @riedgar-ms.
-- [#83](https://github.com/luolingchun/flask-openapi3/pull/83) Be able to change 422 validation errors to other http response status. Thanks, @CostcoFanboy.
-- [#86](https://github.com/luolingchun/flask-openapi3/issues/86) Responses key supports both string, int, and HTTPStatus. Thanks, @CostcoFanboy.
-
-## v2.4.0 2023-06-04
-
-- [#72](https://github.com/luolingchun/flask-openapi3/pull/72) security_schemes(SecurityScheme) supports a json format.
-- [#68](https://github.com/luolingchun/flask-openapi3/pull/68) feat: Add operation_id_callback. Thanks, @BoyanYK.
-- [#64](https://github.com/luolingchun/flask-openapi3/pull/64) Explains the usage of flask openapi command more clearly. Thanks, @candleindark.
-- [#75](https://github.com/luolingchun/flask-openapi3/pull/75) Init view_class and pass view_kwargs. Thanks, @stufisher.
-- [#70](https://github.com/luolingchun/flask-openapi3/issues/70) Support for Specification Extensions in OpenAPI Object and Operation Object. Thanks, @simonblund.
-- [#73](https://github.com/luolingchun/flask-openapi3/issues/73) BaseModel Config support openapi_extra.
-- Merge `extra_responses` to `responses` and deprecate `extra_responses`.
-
-**DeprecationWarning:**
-
-- Add DeprecationWarning to `APIKey`, `HTTPBase`, `OAuth2`, `OpenIdConnect`, `HTTPBearer` that will be deprecated in v3.0.
-- Add DeprecationWarning to `extra_form`, `extra_body` and `extra_responses` that will be deprecated in v3.0.
-
-
-## v2.3.2 2023-04-03
-
-- [#61](https://github.com/luolingchun/flask-openapi3/issues/61) Fix headers with pydantic alias
-
-## v2.3.1 2023-02-13
-
-- remove * in install_requires for setuptools 67+
-
-## v2.3.0 2023-02-12
-
-- Support for custom UI templates (#55)
-- endpoint index rename to openapi
-- fix missing enum in component schemas
-
-## v2.2.2 2023-01-01
-
-- Fix async
-- Fix duplicate tags
-
-## v2.2.1 2022-11-23
-
-- Add dependent files
-
-## v2.2.0 2022-11-14
-
-- support APIView
-- Add mypy
-- Support for python 3.11
-- Upgrade Swagger UI 4.15.5
-- Upgrade Redoc UI 2.0.0
-
-## v2.1.1 2022-10-12
-
-- [#41](https://github.com/luolingchun/flask-openapi3/issues/41) Set the `requestBody required` default value to True. Thanks, @Colin-b
-- Fix multi decorator for api
-- [#42](https://github.com/luolingchun/flask-openapi3/issues/42) Fix required header is not found when `_` in header field. Thanks, @elirud
-
-## v2.1.0 2022-09-04
-
-- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_form for operation. Thanks, @Colin-b
-- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_body for operation. Thanks, @Colin-b
-- Add external_docs for operation
-- Add servers for operation
-- Support to parse extra field in parameters
-- [#35](https://github.com/luolingchun/flask-openapi3/issues/35) Fixed extra_responses can now be used to set every field in Response. Thanks, @Colin-b
-- Upgrade Swagger UI 4.14.0
-- Upgrade Redoc UI 2.0.0-rc.76
-- Upgrade RapiDoc UI 9.3.3
-
-
-### Breaking Changes
-
-- [#39](https://github.com/luolingchun/flask-openapi3/issues/39) Remove configuration FLASK_OPENAPI_VALIDATE_RESPONSE
-
-
-## v2.0.1 2022-08-07
-
-- [#32](https://github.com/luolingchun/flask-openapi3/issues/32) Fix: parse_rule is deprecated in werkzeug>=2.2.0.
-
-## v2.0.0 2022-06-26
-
-- [#26](https://github.com/luolingchun/flask-openapi3/issues/26) Fixed: Body throws exception when receiving str instead of dict. Thanks, @nor3th
-- [#23](https://github.com/luolingchun/flask-openapi3/pull/23) Fixed externalDocs support. Thanks, @dvaerum
-- [#28](https://github.com/luolingchun/flask-openapi3/pull/28) Fixed to enable `__root__` property when validation responses. Thanks, @dvaerum
-- [#17](https://github.com/luolingchun/flask-openapi3/issues/17) Support for Nested APIBlueprint enhancement. Thanks, @dvaerum
-- [#29](https://github.com/luolingchun/flask-openapi3/pull/29) Support disable warnings. Thanks, @dvaerum
-- Support for empty response body. Thanks, @dvaerum
-- Support reload authorizations in Swagger UI
-- Add `flask openapi` command
-- Add options in view functions
-- Upgrade flask to v2.x
-
-### Breaking Changes
-
-- Remove export markdown to `flask openapi` command
-- Configuration `VALIDATE_RESPONSE` rename to `FLASK_OPENAPI_VALIDATE_RESPONSE`
-
-## v1.1.4 2022-05-05
-
-- fix: Trailing slash in APIBlueprint
-
-## v1.1.3 2022-05-01
-
-- fix: Find globalns for the unwrapped func
-- [#19](https://github.com/luolingchun/flask-openapi3/issues/19) fix: Trailing slash in APIBlueprint. Thanks, @ev-agelos
-- add description for UnprocessableEntity
-- remove printouts in `__init__.py`
-
-## v1.1.2 2022-04-01
-
-- [#16](https://github.com/luolingchun/flask-openapi3/issues/16) Fix fileStorage list is not supported. Thanks, @tekrei
-
-## v1.1.0 2022-03-13
-
-- [#13](https://github.com/luolingchun/flask-openapi3/issues/13) drop support for flask 1.0.x. Thanks, @danmur
-- [#15](https://github.com/luolingchun/flask-openapi3/pull/15) Fix to enable BaseModel with `__root__` property. Thanks, @tarcisiojr
-- [#14](https://github.com/luolingchun/flask-openapi3/pull/14) Custom parameters: doc_prefix, api_doc_url, swagger_url, redoc_url, rapidoc_url. Thanks, @barryrobison
-- Upgrade swagger UI v4.6.2
-- Upgrade Redoc v2.0.0-rc.63
-- Upgrade RapiDoc v9.2.0
-
-## v1.0.1 2022-02-12
-
-- add operation_id for OpenAPI Specification
-
-## v1.0.0 2022-01-11
-
-- [#10](https://github.com/luolingchun/flask-openapi3/issues/10) Fix: header's title case. Thanks, @rrr34
-- [#9](https://github.com/luolingchun/flask-openapi3/issues/9) Support for extra responses. Thanks, @blynn99
-- [#12](https://github.com/luolingchun/flask-openapi3/pull/12) Support for path operation field deprecated. Thanks, @blynn99
-- Add keyword parameters `summary` and `description`
-- Add servers for OpenAPI
-- Upgrade swagger UI v4.1.3
-- Upgrade Redoc v2.0.0-rc.59
-- Add rapidoc
-
-### Breaking Changes
-
-- Renamed `securitySchemes` to `security_schemes`
-- Renamed `docExpansion` to `doc_expansion`
-
-## v0.9.9 2021-12-09
-
-- fix: default value in a query and form model
-- fix: empty form and body
-- support `from __future__ import annotations`
-- drop python36
-
-## v0.9.8 2021-11-12
-
-- add Configuration `docExpansion`
-- query and form add array support
-
-## v0.9.7 2021-08-19
-
-- fix: path $ref
-- fix: markdown enum
-
-## v0.9.6 2021-08-18
-
-- Export to markdown(Experimental)
-
-## v0.9.5 2021-07-11
-
-- remove `validate_resp` and add `VALIDATE_RESPONSE`
-
-## v0.9.4 2021-07-03
-
-- OpenAPI add responses and APIBlueprint add abp_responses
-- fix: validate response error when responses is empty dict
-- [#3](https://github.com/luolingchun/flask-openapi3/issues/3) endpoint and APIBlueprint add `doc_ui`. Thanks, @DerManoMann
-- [#4](https://github.com/luolingchun/flask-openapi3/issues/4) fix: response description. Thanks, @DerManoMann
-- [#5](https://github.com/luolingchun/flask-openapi3/issues/5) add custom parameter `oauth_config`. Thanks, @DerManoMann
-- [#6](https://github.com/luolingchun/flask-openapi3/issues/6) support validation Flask Response. Thanks, @DerManoMann
-- [#7](https://github.com/luolingchun/flask-openapi3/issues/7) fix: response validation does not work when uses
-  http.HTTPStatus enums as status_code. Thanks, @DerManoMann
-
-## v0.9.3 2021-06-08
-
-- APIBlueprint adds abp_tags and abp_security
-- fix: tags de-duplication
-- fix: operation summary and description
-
-## v0.9.2 2021-05-17
-
-- fix: _do_decorator
-- add doc_ui args. support close swagger UI and redoc
-
-## v0.9.1 2021-05-16
-
-- fix：request data is None
-- json-->body
-- set 422 Content-Type application/json
-- raise response validate exception
-- fix: TypeError: issubclass() arg 1 must be a class
-
-## v0.9.0 2021-05-13
-
-- first version
+## v3.1.1 2024-04-21
+
+- Wrong types of exclusiveMinimum & exclusiveMaximum fields in Schema class by @Lavertis in #149
+
+## v3.1.0 2024-03-24
+
+- Add the swagger_config parameter to configure the swagger ui by @luolingchun in #146
+- Use full links in Swagger and RapiDoc
+- Upgrade Redoc to 2.1.3
+- Upgrade Swagger to 5.12.0
+
+**DeprecationWarning**
+
+- The doc_expansion parameter is deprecated; use swagger_config instead.
+
+## v3.0.2 2024-01-28
+
+- Fix missing Pydantic Calculated Fields (#141). Thanks, @thebmw.
+
+## v3.0.1 2023-11-26
+
+- Fix the same operationId in APIBlueprint (#133). Thanks, @fluffybrain3.
+- Make body required false (#130). Thanks, @styper.
+- The default value defined in the form is invalid (#129). Thanks, @seekplum.
+
+## v3.0.0 2023-10-22
+
+- Upgrade pydantic to v2.
+- Remove deprecated code.
+- Drop support for Python 3.7.
+- support for raw requests (#109).
+- Upgrade Swagger UI v5.9.0.
+- Upgrade Redoc v2.1.2
+- Update RapiDoc 9.3.4.
+- [#105](https://github.com/luolingchun/flask-openapi3/pull/105) Supports valid properties only. Thanks, @ota42y.
+- [#106](https://github.com/luolingchun/flask-openapi3/pull/106) Bugfix for parameter object. Thanks, @ota42y.
+- [#107](https://github.com/luolingchun/flask-openapi3/pull/107) Bugfix for generics class. Thanks, @ota42y.
+- [#114](https://github.com/luolingchun/flask-openapi3/pull/114) Support Flask 3.0.
+- [#118](https://github.com/luolingchun/flask-openapi3/discussions/118) Fix missed components schemas in ValidationErrorModel. Thanks, @SeFeX.
+- [#122](https://github.com/luolingchun/flask-openapi3/issues/122) Skip 422 response non parameters. Thanks, @Danielsn1.
+
+
+## v3.0.0rc2 2023-10-03
+
+- [#105](https://github.com/luolingchun/flask-openapi3/pull/105) Supports valid properties only. Thanks, @ota42y.
+- [#106](https://github.com/luolingchun/flask-openapi3/pull/106) Bugfix for parameter object. Thanks, @ota42y.
+- [#107](https://github.com/luolingchun/flask-openapi3/pull/107) Bugfix for generics class. Thanks, @ota42y.
+- [#114](https://github.com/luolingchun/flask-openapi3/pull/114) Support Flask 3.0.
+
+## v3.0.0rc1 2023-09-03
+
+- Upgrade pydantic to v2
+- Remove deprecated code
+- Drop support for Python 3.7
+
+## v2.5.5 2023-11-26
+
+- Fix the same operationId in APIBlueprint (#133). Thanks, @fluffybrain3.
+- Make body required false (#130). Thanks, @styper.
+- The default value defined in the form is invalid (#129). Thanks, @seekplum.
+
+## v2.5.4 2023-10-22
+
+- [#118](https://github.com/luolingchun/flask-openapi3/discussions/118) Fix missed components schemas in ValidationErrorModel. Thanks, @SeFeX.
+- [#122](https://github.com/luolingchun/flask-openapi3/issues/122) Skip 422 response non parameters. Thanks, @Danielsn1.
+
+## v2.5.3 2023-10-03
+
+- [#105](https://github.com/luolingchun/flask-openapi3/pull/105) Supports valid properties only. Thanks, @ota42y.
+- [#106](https://github.com/luolingchun/flask-openapi3/pull/106) Bugfix for parameter object. Thanks, @ota42y.
+- [#107](https://github.com/luolingchun/flask-openapi3/pull/107) Bugfix for generics class. Thanks, @ota42y.
+
+## v2.5.2 2023-08-13
+
+- [#97](https://github.com/luolingchun/flask-openapi3/issues/97) Fix response miss description. Thanks, @tekrei.
+
+## v2.5.1 2023-08-07
+
+- [#95](https://github.com/luolingchun/flask-openapi3/pull/95) Added ability to deserialize complex form parameter objects. Thanks, @BlackGad.
+
+## v2.5.0 2023-08-02
+
+- [#79](https://github.com/luolingchun/flask-openapi3/discussions/79) Support `by_alias` in Model Config. Thanks, @candleindark.
+- [#82](https://github.com/luolingchun/flask-openapi3/issues/82) Fix parameter in url_prefix. Thanks, @riedgar-ms.
+- [#83](https://github.com/luolingchun/flask-openapi3/pull/83) Be able to change 422 validation errors to other http response status. Thanks, @CostcoFanboy.
+- [#86](https://github.com/luolingchun/flask-openapi3/issues/86) Responses key supports both string, int, and HTTPStatus. Thanks, @CostcoFanboy.
+
+## v2.4.0 2023-06-04
+
+- [#72](https://github.com/luolingchun/flask-openapi3/pull/72) security_schemes(SecurityScheme) supports a json format.
+- [#68](https://github.com/luolingchun/flask-openapi3/pull/68) feat: Add operation_id_callback. Thanks, @BoyanYK.
+- [#64](https://github.com/luolingchun/flask-openapi3/pull/64) Explains the usage of flask openapi command more clearly. Thanks, @candleindark.
+- [#75](https://github.com/luolingchun/flask-openapi3/pull/75) Init view_class and pass view_kwargs. Thanks, @stufisher.
+- [#70](https://github.com/luolingchun/flask-openapi3/issues/70) Support for Specification Extensions in OpenAPI Object and Operation Object. Thanks, @simonblund.
+- [#73](https://github.com/luolingchun/flask-openapi3/issues/73) BaseModel Config support openapi_extra.
+- Merge `extra_responses` to `responses` and deprecate `extra_responses`.
+
+**DeprecationWarning:**
+
+- Add DeprecationWarning to `APIKey`, `HTTPBase`, `OAuth2`, `OpenIdConnect`, `HTTPBearer` that will be deprecated in v3.0.
+- Add DeprecationWarning to `extra_form`, `extra_body` and `extra_responses` that will be deprecated in v3.0.
+
+
+## v2.3.2 2023-04-03
+
+- [#61](https://github.com/luolingchun/flask-openapi3/issues/61) Fix headers with pydantic alias
+
+## v2.3.1 2023-02-13
+
+- remove * in install_requires for setuptools 67+
+
+## v2.3.0 2023-02-12
+
+- Support for custom UI templates (#55)
+- endpoint index rename to openapi
+- fix missing enum in component schemas
+
+## v2.2.2 2023-01-01
+
+- Fix async
+- Fix duplicate tags
+
+## v2.2.1 2022-11-23
+
+- Add dependent files
+
+## v2.2.0 2022-11-14
+
+- support APIView
+- Add mypy
+- Support for python 3.11
+- Upgrade Swagger UI 4.15.5
+- Upgrade Redoc UI 2.0.0
+
+## v2.1.1 2022-10-12
+
+- [#41](https://github.com/luolingchun/flask-openapi3/issues/41) Set the `requestBody required` default value to True. Thanks, @Colin-b
+- Fix multi decorator for api
+- [#42](https://github.com/luolingchun/flask-openapi3/issues/42) Fix required header is not found when `_` in header field. Thanks, @elirud
+
+## v2.1.0 2022-09-04
+
+- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_form for operation. Thanks, @Colin-b
+- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_body for operation. Thanks, @Colin-b
+- Add external_docs for operation
+- Add servers for operation
+- Support to parse extra field in parameters
+- [#35](https://github.com/luolingchun/flask-openapi3/issues/35) Fixed extra_responses can now be used to set every field in Response. Thanks, @Colin-b
+- Upgrade Swagger UI 4.14.0
+- Upgrade Redoc UI 2.0.0-rc.76
+- Upgrade RapiDoc UI 9.3.3
+
+
+### Breaking Changes
+
+- [#39](https://github.com/luolingchun/flask-openapi3/issues/39) Remove configuration FLASK_OPENAPI_VALIDATE_RESPONSE
+
+
+## v2.0.1 2022-08-07
+
+- [#32](https://github.com/luolingchun/flask-openapi3/issues/32) Fix: parse_rule is deprecated in werkzeug>=2.2.0.
+
+## v2.0.0 2022-06-26
+
+- [#26](https://github.com/luolingchun/flask-openapi3/issues/26) Fixed: Body throws exception when receiving str instead of dict. Thanks, @nor3th
+- [#23](https://github.com/luolingchun/flask-openapi3/pull/23) Fixed externalDocs support. Thanks, @dvaerum
+- [#28](https://github.com/luolingchun/flask-openapi3/pull/28) Fixed to enable `__root__` property when validation responses. Thanks, @dvaerum
+- [#17](https://github.com/luolingchun/flask-openapi3/issues/17) Support for Nested APIBlueprint enhancement. Thanks, @dvaerum
+- [#29](https://github.com/luolingchun/flask-openapi3/pull/29) Support disable warnings. Thanks, @dvaerum
+- Support for empty response body. Thanks, @dvaerum
+- Support reload authorizations in Swagger UI
+- Add `flask openapi` command
+- Add options in view functions
+- Upgrade flask to v2.x
+
+### Breaking Changes
+
+- Remove export markdown to `flask openapi` command
+- Configuration `VALIDATE_RESPONSE` rename to `FLASK_OPENAPI_VALIDATE_RESPONSE`
+
+## v1.1.4 2022-05-05
+
+- fix: Trailing slash in APIBlueprint
+
+## v1.1.3 2022-05-01
+
+- fix: Find globalns for the unwrapped func
+- [#19](https://github.com/luolingchun/flask-openapi3/issues/19) fix: Trailing slash in APIBlueprint. Thanks, @ev-agelos
+- add description for UnprocessableEntity
+- remove printouts in `__init__.py`
+
+## v1.1.2 2022-04-01
+
+- [#16](https://github.com/luolingchun/flask-openapi3/issues/16) Fix fileStorage list is not supported. Thanks, @tekrei
+
+## v1.1.0 2022-03-13
+
+- [#13](https://github.com/luolingchun/flask-openapi3/issues/13) drop support for flask 1.0.x. Thanks, @danmur
+- [#15](https://github.com/luolingchun/flask-openapi3/pull/15) Fix to enable BaseModel with `__root__` property. Thanks, @tarcisiojr
+- [#14](https://github.com/luolingchun/flask-openapi3/pull/14) Custom parameters: doc_prefix, api_doc_url, swagger_url, redoc_url, rapidoc_url. Thanks, @barryrobison
+- Upgrade swagger UI v4.6.2
+- Upgrade Redoc v2.0.0-rc.63
+- Upgrade RapiDoc v9.2.0
+
+## v1.0.1 2022-02-12
+
+- add operation_id for OpenAPI Specification
+
+## v1.0.0 2022-01-11
+
+- [#10](https://github.com/luolingchun/flask-openapi3/issues/10) Fix: header's title case. Thanks, @rrr34
+- [#9](https://github.com/luolingchun/flask-openapi3/issues/9) Support for extra responses. Thanks, @blynn99
+- [#12](https://github.com/luolingchun/flask-openapi3/pull/12) Support for path operation field deprecated. Thanks, @blynn99
+- Add keyword parameters `summary` and `description`
+- Add servers for OpenAPI
+- Upgrade swagger UI v4.1.3
+- Upgrade Redoc v2.0.0-rc.59
+- Add rapidoc
+
+### Breaking Changes
+
+- Renamed `securitySchemes` to `security_schemes`
+- Renamed `docExpansion` to `doc_expansion`
+
+## v0.9.9 2021-12-09
+
+- fix: default value in a query and form model
+- fix: empty form and body
+- support `from __future__ import annotations`
+- drop python36
+
+## v0.9.8 2021-11-12
+
+- add Configuration `docExpansion`
+- query and form add array support
+
+## v0.9.7 2021-08-19
+
+- fix: path $ref
+- fix: markdown enum
+
+## v0.9.6 2021-08-18
+
+- Export to markdown(Experimental)
+
+## v0.9.5 2021-07-11
+
+- remove `validate_resp` and add `VALIDATE_RESPONSE`
+
+## v0.9.4 2021-07-03
+
+- OpenAPI add responses and APIBlueprint add abp_responses
+- fix: validate response error when responses is empty dict
+- [#3](https://github.com/luolingchun/flask-openapi3/issues/3) endpoint and APIBlueprint add `doc_ui`. Thanks, @DerManoMann
+- [#4](https://github.com/luolingchun/flask-openapi3/issues/4) fix: response description. Thanks, @DerManoMann
+- [#5](https://github.com/luolingchun/flask-openapi3/issues/5) add custom parameter `oauth_config`. Thanks, @DerManoMann
+- [#6](https://github.com/luolingchun/flask-openapi3/issues/6) support validation Flask Response. Thanks, @DerManoMann
+- [#7](https://github.com/luolingchun/flask-openapi3/issues/7) fix: response validation does not work when uses
+  http.HTTPStatus enums as status_code. Thanks, @DerManoMann
+
+## v0.9.3 2021-06-08
+
+- APIBlueprint adds abp_tags and abp_security
+- fix: tags de-duplication
+- fix: operation summary and description
+
+## v0.9.2 2021-05-17
+
+- fix: _do_decorator
+- add doc_ui args. support close swagger UI and redoc
+
+## v0.9.1 2021-05-16
+
+- fix：request data is None
+- json-->body
+- set 422 Content-Type application/json
+- raise response validate exception
+- fix: TypeError: issubclass() arg 1 must be a class
+
+## v0.9.0 2021-05-13
+
+- first version
```

### Comparing `flask_openapi3-3.1.1/CONTRIBUTING.md` & `flask_openapi3-4.0.0.dev0/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-## Contributing Guide
-
-Thank you for contributing to Flask OpenAPI3.
-
-1. [Create a new issue](https://github.com/luolingchun/flask-openapi3/issues/new)
-2. [Fork and Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
-
-Before submitting pr, you need to complete the following steps:
-
-1. Install requirements
-
-    ```bash
-    pip install -U flask pydantic
-    ```
-
-2. Running the tests
-
-    ```bash
-    set pythonpath=. 
-    # or export pythonpath=.
-    pytest tests
-    ```
-
-3. Running the flake8
-
-    ```bash
-    flake8 flask_openapi3 tests examples
-    ```
-
-4. Running the mypy
-
-    ```bash
-    mypy flask_openapi3
-    ```
-
-5. Building the docs
-
-    Serve the live docs with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material), and make sure it's correct.
-
-    ```bash
-    mkdocs serve
-    ```
+## Contributing Guide
+
+Thank you for contributing to Flask OpenAPI3.
+
+1. [Create a new issue](https://github.com/luolingchun/flask-openapi3/issues/new)
+2. [Fork and Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
+
+Before submitting pr, you need to complete the following steps:
+
+1. Install requirements
+
+    ```bash
+    pip install -U flask pydantic
+    ```
+
+2. Running the tests
+
+    ```bash
+    set pythonpath=. 
+    # or export pythonpath=.
+    pytest tests
+    ```
+
+3. Running the flake8
+
+    ```bash
+    flake8 flask_openapi3 tests examples
+    ```
+
+4. Running the mypy
+
+    ```bash
+    mypy flask_openapi3
+    ```
+
+5. Building the docs
+
+    Serve the live docs with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material), and make sure it's correct.
+
+    ```bash
+    mkdocs serve
+    ```
```

### Comparing `flask_openapi3-3.1.1/examples/async_demo.py` & `flask_openapi3-4.0.0.dev0/examples/async_demo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/11/30 14:55
-
-from typing import Optional
-
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import OpenAPI, APIView
-
-app = OpenAPI(__name__)
-api_view = APIView(url_prefix="/api/v1")
-
-
-class Query(BaseModel):
-    q: str
-
-
-class BookQuery(BaseModel):
-    age: Optional[int] = Field(None, description='Age')
-
-
-class BookBody(BaseModel):
-    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
-    author: str = Field(None, min_length=2, max_length=4, description='Author')
-
-
-@app.get('/open/api')
-async def get_openapi(query: Query):
-    print(query)
-    return 'GET, OpenAPI!'
-
-
-@app.post('/open/api')
-async def post_openapi(body: Query):
-    print(body)
-    return 'POST, OpenAPI!'
-
-
-@api_view.route("/book")
-class BookListAPIView:
-
-    @api_view.doc(summary="get book list")
-    async def get(self, query: BookQuery):
-        return query.model_dump_json()
-
-    @api_view.doc(summary="create book")
-    async def post(self, body: BookBody):
-        """description for a created book"""
-        return body.model_dump_json()
-
-
-app.register_api_view(api_view)
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/11/30 14:55
+
+from typing import Optional
+
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import OpenAPI, APIView
+
+app = OpenAPI(__name__)
+api_view = APIView(url_prefix="/api/v1")
+
+
+class Query(BaseModel):
+    q: str
+
+
+class BookQuery(BaseModel):
+    age: Optional[int] = Field(None, description='Age')
+
+
+class BookBody(BaseModel):
+    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
+    author: str = Field(None, min_length=2, max_length=4, description='Author')
+
+
+@app.get('/open/api')
+async def get_openapi(query: Query):
+    print(query)
+    return 'GET, OpenAPI!'
+
+
+@app.post('/open/api')
+async def post_openapi(body: Query):
+    print(body)
+    return 'POST, OpenAPI!'
+
+
+@api_view.route("/book")
+class BookListAPIView:
+
+    @api_view.doc(summary="get book list")
+    async def get(self, query: BookQuery):
+        return query.model_dump_json()
+
+    @api_view.doc(summary="create book")
+    async def post(self, body: BookBody):
+        """description for a created book"""
+        return body.model_dump_json()
+
+
+app.register_api_view(api_view)
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/custom_ui_templates_demo.py` & `flask_openapi3-4.0.0.dev0/examples/custom_ui_templates_demo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/2/3 15:14
-from pydantic import BaseModel
-
-from flask_openapi3 import Info, Tag
-from flask_openapi3 import OpenAPI
-
-info = Info(title="book API", version="1.0.0")
-swagger_html_string = """
-<!DOCTYPE html>
-<html lang="en">
-<head>
-    <meta charset="UTF-8">
-    <title>Custom Title</title>
-    <link rel="stylesheet" type="text/css" href="https://unpkg.com/swagger-ui-dist/swagger-ui.css">
-    <style>
-        html {
-            box-sizing: border-box;
-            overflow: -moz-scrollbars-vertical;
-            overflow-y: scroll;
-        }
-
-        *, *:before, *:after {
-            box-sizing: inherit;
-        }
-
-        body {
-            margin: 0;
-            background: #fafafa;
-        }
-    </style>
-</head>
-<body>
-<div id="swagger-ui"></div>
-<script src="https://unpkg.com/swagger-ui-dist/swagger-ui-bundle.js"></script>
-<script src="https://unpkg.com/swagger-ui-dist/swagger-ui-standalone-preset.js"></script>
-<script>
-    window.onload = function () {
-        // Begin Swagger UI call region
-        window.ui = SwaggerUIBundle({
-            url: "{{api_doc_url}}",
-            dom_id: "#swagger-ui",
-            deepLinking: true,
-            presets: [
-                SwaggerUIBundle.presets.apis,
-                SwaggerUIStandalonePreset
-            ],
-            plugins: [
-                SwaggerUIBundle.plugins.DownloadUrl
-            ],
-            layout: "StandaloneLayout"
-        })
-    }
-</script>
-</body>
-</html>
-"""
-
-rapipdf_html_string = """
-<!doctype html>
-  <html>
-  <head>
-    <script src="https://unpkg.com/rapipdf/dist/rapipdf-min.js"></script>
-  </head>
-  <body>
-    <rapi-pdf
-      style = "width:700px; height:40px; font-size:18px;"
-      spec-url = "{{api_doc_url}}"
-      button-bg = "#b44646"
-    > </rapi-pdf>
-  </body>
-  </html>
-"""
-ui_templates = {
-    "swagger": swagger_html_string,
-    "rapipdf": rapipdf_html_string
-}
-app = OpenAPI(__name__, info=info, ui_templates=ui_templates)
-
-book_tag = Tag(name='book', description='Some Book')
-
-
-class BookQuery(BaseModel):
-    age: int
-    author: str
-
-
-@app.get('/book', tags=[book_tag])
-def get_book(query: BookQuery):
-    """get books
-    to get all books
-    """
-    return {
-        "code": 0,
-        "message": "ok",
-        "data": [
-            {"bid": 1, "age": query.age, "author": query.author},
-            {"bid": 2, "age": query.age, "author": query.author}
-        ]
-    }
-
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/2/3 15:14
+from pydantic import BaseModel
+
+from flask_openapi3 import Info, Tag
+from flask_openapi3 import OpenAPI
+
+info = Info(title="book API", version="1.0.0")
+swagger_html_string = """
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <title>Custom Title</title>
+    <link rel="stylesheet" type="text/css" href="https://unpkg.com/swagger-ui-dist/swagger-ui.css">
+    <style>
+        html {
+            box-sizing: border-box;
+            overflow: -moz-scrollbars-vertical;
+            overflow-y: scroll;
+        }
+
+        *, *:before, *:after {
+            box-sizing: inherit;
+        }
+
+        body {
+            margin: 0;
+            background: #fafafa;
+        }
+    </style>
+</head>
+<body>
+<div id="swagger-ui"></div>
+<script src="https://unpkg.com/swagger-ui-dist/swagger-ui-bundle.js"></script>
+<script src="https://unpkg.com/swagger-ui-dist/swagger-ui-standalone-preset.js"></script>
+<script>
+    window.onload = function () {
+        // Begin Swagger UI call region
+        window.ui = SwaggerUIBundle({
+            url: "{{api_doc_url}}",
+            dom_id: "#swagger-ui",
+            deepLinking: true,
+            presets: [
+                SwaggerUIBundle.presets.apis,
+                SwaggerUIStandalonePreset
+            ],
+            plugins: [
+                SwaggerUIBundle.plugins.DownloadUrl
+            ],
+            layout: "StandaloneLayout"
+        })
+    }
+</script>
+</body>
+</html>
+"""
+
+rapipdf_html_string = """
+<!doctype html>
+  <html>
+  <head>
+    <script src="https://unpkg.com/rapipdf/dist/rapipdf-min.js"></script>
+  </head>
+  <body>
+    <rapi-pdf
+      style = "width:700px; height:40px; font-size:18px;"
+      spec-url = "{{api_doc_url}}"
+      button-bg = "#b44646"
+    > </rapi-pdf>
+  </body>
+  </html>
+"""
+ui_templates = {
+    "swagger": swagger_html_string,
+    "rapipdf": rapipdf_html_string
+}
+app = OpenAPI(__name__, info=info, ui_templates=ui_templates)
+
+book_tag = Tag(name='book', description='Some Book')
+
+
+class BookQuery(BaseModel):
+    age: int
+    author: str
+
+
+@app.get('/book', tags=[book_tag])
+def get_book(query: BookQuery):
+    """get books
+    to get all books
+    """
+    return {
+        "code": 0,
+        "message": "ok",
+        "data": [
+            {"bid": 1, "age": query.age, "author": query.author},
+            {"bid": 2, "age": query.age, "author": query.author}
+        ]
+    }
+
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/header_demo.py` & `flask_openapi3-4.0.0.dev0/examples/header_demo.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/12/26 15:07
-
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import Info, Tag
-from flask_openapi3 import OpenAPI
-
-info = Info(title='header API', version='1.0.0')
-app = OpenAPI(__name__, info=info)
-
-book_tag = Tag(name='book', description='Some Book')
-
-
-class Headers(BaseModel):
-    hello: str = Field("what's up", max_length=12, description='sds')
-    # required
-    # hello: str = Field(..., max_length=12, description='sds')
-    x_hello: str = Field(..., max_length=12, description='Header with alias to support dash', alias="x-hello")
-
-
-@app.get('/book', tags=[book_tag])
-def get_book(header: Headers):
-    print(header)
-    return header.hello
-
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/12/26 15:07
+
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import Info, Tag
+from flask_openapi3 import OpenAPI
+
+info = Info(title='header API', version='1.0.0')
+app = OpenAPI(__name__, info=info)
+
+book_tag = Tag(name='book', description='Some Book')
+
+
+class Headers(BaseModel):
+    hello: str = Field("what's up", max_length=12, description='sds')
+    # required
+    # hello: str = Field(..., max_length=12, description='sds')
+    x_hello: str = Field(..., max_length=12, description='Header with alias to support dash', alias="x-hello")
+
+
+@app.get('/book', tags=[book_tag])
+def get_book(header: Headers):
+    print(header)
+    return header.hello
+
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/init_oauth_demo.py` & `flask_openapi3-4.0.0.dev0/examples/init_oauth_demo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/6/21 11:23
-from flask_openapi3 import Info
-from flask_openapi3 import OpenAPI, OAuthConfig
-
-info = Info(title='oauth API', version='1.0.0')
-
-oauth_config = OAuthConfig(
-    clientId="xxx",
-    clientSecret="xxx"
-)
-
-oauth2 = {
-    "type": "oauth2",
-    "flows": {
-        "implicit": {
-            "authorizationUrl": "https://example.com/api/oauth/dialog",
-            "scopes": {
-                "write:pets": "modify pets in your account",
-                "read:pets": "read your pets"
-            }
-        }
-    }
-}
-security_schemes = {"oauth2": oauth2}
-
-app = OpenAPI(__name__, info=info, oauth_config=oauth_config, security_schemes=security_schemes)
-
-security = [
-    {"oauth2": ["write:pets", "read:pets"]}
-]
-
-
-@app.get("/", security=security)
-def oauth():
-    return "oauth"
-
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/6/21 11:23
+from flask_openapi3 import Info
+from flask_openapi3 import OpenAPI, OAuthConfig
+
+info = Info(title='oauth API', version='1.0.0')
+
+oauth_config = OAuthConfig(
+    clientId="xxx",
+    clientSecret="xxx"
+)
+
+oauth2 = {
+    "type": "oauth2",
+    "flows": {
+        "implicit": {
+            "authorizationUrl": "https://example.com/api/oauth/dialog",
+            "scopes": {
+                "write:pets": "modify pets in your account",
+                "read:pets": "read your pets"
+            }
+        }
+    }
+}
+security_schemes = {"oauth2": oauth2}
+
+app = OpenAPI(__name__, info=info, oauth_config=oauth_config, security_schemes=security_schemes)
+
+security = [
+    {"oauth2": ["write:pets", "read:pets"]}
+]
+
+
+@app.get("/", security=security)
+def oauth():
+    return "oauth"
+
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/nested_apiblueprint_demo.py` & `flask_openapi3-4.0.0.dev0/examples/nested_apiblueprint_demo.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from flask_openapi3 import OpenAPI, APIBlueprint
-
-app = OpenAPI(__name__)
-
-api = APIBlueprint('book', __name__, url_prefix='/api/book')
-api_english = APIBlueprint('english', __name__)
-api_chinese = APIBlueprint('chinese', __name__)
-
-
-@api_english.post('/english')
-def create_english_book():
-    return {"message": "english"}
-
-
-@api_chinese.post('/chinese')
-def create_chinese_book():
-    return {"message": "chinese"}
-
-
-# register nested api
-api.register_api(api_english)
-api.register_api(api_chinese)
-# register api
-app.register_api(api)
-
-if __name__ == '__main__':
-    app.run(debug=True)
+from flask_openapi3 import OpenAPI, APIBlueprint
+
+app = OpenAPI(__name__)
+
+api = APIBlueprint('book', __name__, url_prefix='/api/book')
+api_english = APIBlueprint('english', __name__)
+api_chinese = APIBlueprint('chinese', __name__)
+
+
+@api_english.post('/english')
+def create_english_book():
+    return {"message": "english"}
+
+
+@api_chinese.post('/chinese')
+def create_chinese_book():
+    return {"message": "chinese"}
+
+
+# register nested api
+api.register_api(api_english)
+api.register_api(api_chinese)
+# register api
+app.register_api(api)
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/rest_demo.py` & `flask_openapi3-4.0.0.dev0/examples/rest_demo.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/4/28 11:24
-from http import HTTPStatus
-from typing import Optional, List
-
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import ExternalDocumentation
-from flask_openapi3 import Info, Tag, Server
-from flask_openapi3 import OpenAPI
-
-info = Info(title='book API', version='1.0.0')
-
-# Basic Authentication Sample
-basic = {
-    "type": "http",
-    "scheme": "basic"
-}
-# JWT Bearer Sample
-jwt = {
-    "type": "http",
-    "scheme": "bearer",
-    "bearerFormat": "JWT"
-}
-# API Key Sample
-api_key = {
-    "type": "apiKey",
-    "name": "api_key",
-    "in": "header"
-}
-# Implicit OAuth2 Sample
-oauth2 = {
-    "type": "oauth2",
-    "flows": {
-        "implicit": {
-            "authorizationUrl": "https://example.com/api/oauth/dialog",
-            "scopes": {
-                "write:pets": "modify pets in your account",
-                "read:pets": "read your pets"
-            }
-        }
-    }
-}
-security_schemes = {"jwt": jwt, "api_key": api_key, "oauth2": oauth2, "basic": basic}
-
-
-class NotFoundResponse(BaseModel):
-    code: int = Field(-1, description="Status Code")
-    message: str = Field("Resource not found!", description="Exception Information")
-
-
-app = OpenAPI(__name__, info=info, security_schemes=security_schemes, responses={404: NotFoundResponse})
-
-book_tag = Tag(name='book', description='Some Book')
-security = [
-    {"jwt": []},
-    {"oauth2": ["write:pets", "read:pets"]},
-    {"basic": []}
-]
-
-
-class BookPath(BaseModel):
-    bid: int = Field(..., description='book id', json_schema_extra={"deprecated": True, "example": 100})
-
-
-class BookQuery(BaseModel):
-    age: Optional[int] = Field(None, description='Age')
-    s_list: List[str] = Field(None, alias='s_list[]', description='some array')
-
-
-class BookBody(BaseModel):
-    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
-    author: str = Field(None, min_length=2, max_length=4, description='Author')
-
-
-class BookBodyWithID(BaseModel):
-    bid: int = Field(..., description='book id')
-    age: Optional[int] = Field(None, ge=2, le=4, description='Age')
-    author: str = Field(None, min_length=2, max_length=4, description='Author')
-
-
-class BookResponse(BaseModel):
-    code: int = Field(0, description="Status Code")
-    message: str = Field("ok", description="Exception Information")
-    data: Optional[BookBodyWithID]
-
-
-@app.get(
-    '/book/<int:bid>',
-    tags=[book_tag],
-    summary='new summary',
-    description='new description',
-    operation_id="get_book_id",
-    external_docs=ExternalDocumentation(
-        url="https://www.openapis.org/",
-        description="Something great got better, get excited!"),
-    responses={200: BookResponse},
-    security=security,
-    servers=[Server(url="https://www.openapis.org/", description="openapi")]
-)
-def get_book(path: BookPath):
-    """Get a book
-    to Get some book by id, like:
-    http://localhost:5000/book/3
-    """
-    if path.bid == 4:
-        return NotFoundResponse().model_dump(), 404
-    return {"code": 0, "message": "ok", "data": {"bid": path.bid, "age": 3, "author": 'no'}}
-
-
-# set doc_ui False disable openapi UI
-@app.get('/book', doc_ui=True, deprecated=True)
-def get_books(query: BookQuery):
-    """get books
-    to get all books
-    """
-    print(query)
-    return {
-        "code": 0,
-        "message": "ok",
-        "data": [
-            {"bid": 1, "age": query.age, "author": 'a1'},
-            {"bid": 2, "age": query.age, "author": 'a2'}
-        ]
-    }
-
-
-@app.post('/book', tags=[book_tag], responses={200: BookResponse})
-def create_book(body: BookBody):
-    print(body)
-    return {"code": 0, "message": "ok"}, HTTPStatus.OK
-
-
-@app.put('/book/<int:bid>', tags=[book_tag])
-def update_book(path: BookPath, body: BookBody):
-    print(path)
-    print(body)
-    return {"code": 0, "message": "ok"}
-
-
-@app.delete('/book/<int:bid>', tags=[book_tag], doc_ui=False)
-def delete_book(path: BookPath):
-    print(path)
-    return {"code": 0, "message": "ok"}
-
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/4/28 11:24
+from http import HTTPStatus
+from typing import Optional, List
+
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import ExternalDocumentation
+from flask_openapi3 import Info, Tag, Server
+from flask_openapi3 import OpenAPI
+
+info = Info(title='book API', version='1.0.0')
+
+# Basic Authentication Sample
+basic = {
+    "type": "http",
+    "scheme": "basic"
+}
+# JWT Bearer Sample
+jwt = {
+    "type": "http",
+    "scheme": "bearer",
+    "bearerFormat": "JWT"
+}
+# API Key Sample
+api_key = {
+    "type": "apiKey",
+    "name": "api_key",
+    "in": "header"
+}
+# Implicit OAuth2 Sample
+oauth2 = {
+    "type": "oauth2",
+    "flows": {
+        "implicit": {
+            "authorizationUrl": "https://example.com/api/oauth/dialog",
+            "scopes": {
+                "write:pets": "modify pets in your account",
+                "read:pets": "read your pets"
+            }
+        }
+    }
+}
+security_schemes = {"jwt": jwt, "api_key": api_key, "oauth2": oauth2, "basic": basic}
+
+
+class NotFoundResponse(BaseModel):
+    code: int = Field(-1, description="Status Code")
+    message: str = Field("Resource not found!", description="Exception Information")
+
+
+app = OpenAPI(__name__, info=info, security_schemes=security_schemes, responses={404: NotFoundResponse})
+
+book_tag = Tag(name='book', description='Some Book')
+security = [
+    {"jwt": []},
+    {"oauth2": ["write:pets", "read:pets"]},
+    {"basic": []}
+]
+
+
+class BookPath(BaseModel):
+    bid: int = Field(..., description='book id', json_schema_extra={"deprecated": True, "example": 100})
+
+
+class BookQuery(BaseModel):
+    age: Optional[int] = Field(None, description='Age')
+    s_list: List[str] = Field(None, alias='s_list[]', description='some array')
+
+
+class BookBody(BaseModel):
+    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
+    author: str = Field(None, min_length=2, max_length=4, description='Author')
+
+
+class BookBodyWithID(BaseModel):
+    bid: int = Field(..., description='book id')
+    age: Optional[int] = Field(None, ge=2, le=4, description='Age')
+    author: str = Field(None, min_length=2, max_length=4, description='Author')
+
+
+class BookResponse(BaseModel):
+    code: int = Field(0, description="Status Code")
+    message: str = Field("ok", description="Exception Information")
+    data: Optional[BookBodyWithID]
+
+
+@app.get(
+    '/book/<int:bid>',
+    tags=[book_tag],
+    summary='new summary',
+    description='new description',
+    operation_id="get_book_id",
+    external_docs=ExternalDocumentation(
+        url="https://www.openapis.org/",
+        description="Something great got better, get excited!"),
+    responses={200: BookResponse},
+    security=security,
+    servers=[Server(url="https://www.openapis.org/", description="openapi")]
+)
+def get_book(path: BookPath):
+    """Get a book
+    to Get some book by id, like:
+    http://localhost:5000/book/3
+    """
+    if path.bid == 4:
+        return NotFoundResponse().model_dump(), 404
+    return {"code": 0, "message": "ok", "data": {"bid": path.bid, "age": 3, "author": 'no'}}
+
+
+# set doc_ui False disable openapi UI
+@app.get('/book', doc_ui=True, deprecated=True)
+def get_books(query: BookQuery):
+    """get books
+    to get all books
+    """
+    print(query)
+    return {
+        "code": 0,
+        "message": "ok",
+        "data": [
+            {"bid": 1, "age": query.age, "author": 'a1'},
+            {"bid": 2, "age": query.age, "author": 'a2'}
+        ]
+    }
+
+
+@app.post('/book', tags=[book_tag], responses={200: BookResponse})
+def create_book(body: BookBody):
+    print(body)
+    return {"code": 0, "message": "ok"}, HTTPStatus.OK
+
+
+@app.put('/book/<int:bid>', tags=[book_tag])
+def update_book(path: BookPath, body: BookBody):
+    print(path)
+    print(body)
+    return {"code": 0, "message": "ok"}
+
+
+@app.delete('/book/<int:bid>', tags=[book_tag], doc_ui=False)
+def delete_book(path: BookPath):
+    print(path)
+    return {"code": 0, "message": "ok"}
+
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/servers_demo.py` & `flask_openapi3-4.0.0.dev0/examples/servers_demo.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/1/8 14:25
-from pydantic import BaseModel
-
-from flask_openapi3 import Info, Tag
-from flask_openapi3 import OpenAPI, Server
-
-info = Info(title="book API", version="1.0.0")
-servers = [
-    Server(url="http://127.0.0.1:5000"),
-    Server(url="https://127.0.0.1:5000"),
-]
-app = OpenAPI(__name__, info=info, servers=servers)
-
-book_tag = Tag(name="book", description="Some Book")
-
-
-class BookQuery(BaseModel):
-    age: int
-    author: str
-
-
-@app.get("/book", tags=[book_tag])
-def get_book(query: BookQuery):
-    """get books
-    to get all books
-    """
-    return {
-        "code": 0,
-        "message": "ok",
-        "data": [
-            {"bid": 1, "age": query.age, "author": query.author},
-            {"bid": 2, "age": query.age, "author": query.author}
-        ]
-    }
-
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/1/8 14:25
+from pydantic import BaseModel
+
+from flask_openapi3 import Info, Tag
+from flask_openapi3 import OpenAPI, Server
+
+info = Info(title="book API", version="1.0.0")
+servers = [
+    Server(url="http://127.0.0.1:5000"),
+    Server(url="https://127.0.0.1:5000"),
+]
+app = OpenAPI(__name__, info=info, servers=servers)
+
+book_tag = Tag(name="book", description="Some Book")
+
+
+class BookQuery(BaseModel):
+    age: int
+    author: str
+
+
+@app.get("/book", tags=[book_tag])
+def get_book(query: BookQuery):
+    """get books
+    to get all books
+    """
+    return {
+        "code": 0,
+        "message": "ok",
+        "data": [
+            {"bid": 1, "age": query.age, "author": query.author},
+            {"bid": 2, "age": query.age, "author": query.author}
+        ]
+    }
+
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/examples/upload_file_demo.py` & `flask_openapi3-4.0.0.dev0/examples/upload_file_demo.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/5/11 14:03
-
-from typing import List
-
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import OpenAPI, FileStorage
-
-app = OpenAPI(__name__)
-
-
-class UploadFileForm(BaseModel):
-    file: FileStorage
-    file_type: str = Field(None, description="File Type")
-
-
-class UploadFilesForm(BaseModel):
-    files: List[FileStorage]
-    str_list: List[str]
-    int_list: List[int]
-
-
-@app.post('/upload/file')
-def upload_file(form: UploadFileForm):
-    print(form.file.filename)
-    print(form.file_type)
-    form.file.save('test.jpg')
-    return {"code": 0, "message": "ok"}
-
-
-@app.post('/upload/files')
-def upload_files(form: UploadFilesForm):
-    print(form.files)
-    print(form.str_list)
-    print(form.int_list)
-    return {"code": 0, "message": "ok"}
-
-
-if __name__ == '__main__':
-    app.run(debug=True)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/5/11 14:03
+
+from typing import List
+
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import OpenAPI, FileStorage
+
+app = OpenAPI(__name__)
+
+
+class UploadFileForm(BaseModel):
+    file: FileStorage
+    file_type: str = Field(None, description="File Type")
+
+
+class UploadFilesForm(BaseModel):
+    files: List[FileStorage]
+    str_list: List[str]
+    int_list: List[int]
+
+
+@app.post('/upload/file')
+def upload_file(form: UploadFileForm):
+    print(form.file.filename)
+    print(form.file_type)
+    form.file.save('test.jpg')
+    return {"code": 0, "message": "ok"}
+
+
+@app.post('/upload/files')
+def upload_files(form: UploadFilesForm):
+    print(form.files)
+    print(form.str_list)
+    print(form.int_list)
+    return {"code": 0, "message": "ok"}
+
+
+if __name__ == '__main__':
+    app.run(debug=True)
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/__init__.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/4/30 10:14
-
-from .__version__ import __version__
-from .blueprint import APIBlueprint
-from .models import APISpec
-from .models import Components
-from .models import Contact
-from .models import Discriminator
-from .models import Encoding
-from .models import Example
-from .models import ExternalDocumentation
-from .models import FileStorage
-from .models import Header
-from .models import Info
-from .models import License
-from .models import Link
-from .models import MediaType
-from .models import OAuthConfig
-from .models import OAuthFlow
-from .models import OAuthFlows
-from .models import Operation
-from .models import Parameter
-from .models import ParameterInType
-from .models import PathItem
-from .models import RawModel
-from .models import Reference
-from .models import RequestBody
-from .models import Response
-from .models import Schema
-from .models import SecurityScheme
-from .models import Server
-from .models import ServerVariable
-from .models import StyleValues
-from .models import Tag
-from .models import UnprocessableEntity
-from .models import ValidationErrorModel
-from .models import XML
-from .openapi import OpenAPI
-from .view import APIView
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/4/30 10:14
+
+from .__version__ import __version__
+from .blueprint import APIBlueprint
+from .models import APISpec
+from .models import Components
+from .models import Contact
+from .models import Discriminator
+from .models import Encoding
+from .models import Example
+from .models import ExternalDocumentation
+from .models import FileStorage
+from .models import Header
+from .models import Info
+from .models import License
+from .models import Link
+from .models import MediaType
+from .models import OAuthConfig
+from .models import OAuthFlow
+from .models import OAuthFlows
+from .models import Operation
+from .models import Parameter
+from .models import ParameterInType
+from .models import PathItem
+from .models import RawModel
+from .models import Reference
+from .models import RequestBody
+from .models import Response
+from .models import Schema
+from .models import SecurityScheme
+from .models import Server
+from .models import ServerVariable
+from .models import StyleValues
+from .models import Tag
+from .models import UnprocessableEntity
+from .models import ValidationErrorModel
+from .models import XML
+from .openapi import OpenAPI
+from .view import APIView
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/markdown.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/markdown.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/8/11 10:39
-from .models import OPENAPI3_REF_PREFIX
-
-
-def parse_schemas(schemas):
-    schemas_dict = {}
-    for name, obj in schemas.items():
-        schemas_dict[name] = "| name | type | required | description |\n"
-        schemas_dict[name] += "| ---- | ---- | -------- | ----------- |\n"
-        required = obj.get('required', [])
-        enum = obj.get('enum')
-        if enum:
-            schemas_dict[name] += f"| {name} | {obj.get('type', '')} | - | Enum: {', '.join(enum)} |\n"
-        properties = obj.get('properties')
-        if properties:
-            for property_name, _property in properties.items():
-                ref = _property.get('$ref')
-                if ref:
-                    ref_name = ref.lstrip(OPENAPI3_REF_PREFIX + '/')
-                    schemas_dict[name] += f"| {property_name} | - | - | [{ref_name}](#{ref_name}) |\n"
-                else:
-                    schemas_dict[name] += f"| {property_name} " \
-                                          f"| {_property.get('format', '') or _property.get('type', '')} " \
-                                          f"| {property_name in required} " \
-                                          f"| {_property.get('description', '')} " \
-                                          f"|\n"
-    return schemas_dict
-
-
-def parse_parameters(parameters):
-    md = "| name | type | in   | required | description |\n"
-    md += "| ---- | ---- | ---- | -------- | ----------- |\n"
-    for param in parameters:
-        aff_of = param['schema'].get('allOf')
-        if aff_of:
-            for one in aff_of:
-                if isinstance(one, dict) and one.get('$ref'):
-                    ref_name = one.get('$ref').lstrip(OPENAPI3_REF_PREFIX + '/')
-                    md += f"| {param.get('name', '')} " \
-                          f"| {param['schema'].get('type', '')} " \
-                          f"| {param.get('in', '')} " \
-                          f"| {param.get('required', '')} " \
-                          f"| [{ref_name}](#{ref_name}) " \
-                          f"|\n"
-                    break
-            continue
-        md += f"| {param.get('name', '')} " \
-              f"| {param['schema'].get('type', '')} " \
-              f"| {param.get('in', '')} " \
-              f"| {param.get('required', '')} " \
-              f"| {param.get('description', '')} " \
-              f"|\n"
-    md += "\n"
-    return md
-
-
-def parse_request_body(request_body, schemas_dict):
-    md = ''
-    content = request_body['content']
-    for media_type, schemas in content.items():
-        md += f"*{media_type}*\n\n"
-        ref = schemas['schema']['$ref']
-        obj_name = ref.lstrip(OPENAPI3_REF_PREFIX + '/')
-        md += f"{schemas_dict.get(obj_name, '')}"
-    md += "\n"
-    return md
-
-
-def openapi_to_markdown(api_json: dict) -> str:
-    markdown = ''
-    # info and version
-    info = api_json['info']
-    markdown += f"# {info['title']}\n\n"
-    markdown += f"**version**: *{info['version']}*\n\n"
-    # tags
-    tag_dict = {}
-    for tag in api_json.get('tags', []):
-        tag_dict[tag['name']] = {'description': tag['description'], 'paths': ''}
-    if not tag_dict.get('default'):
-        tag_dict['default'] = {'paths': ''}
-    # schemas
-    components = api_json.get("components", {})
-    schemas = components.get('schemas', {})
-    schemas_dict = parse_schemas(schemas)
-    # paths
-    for route, path in api_json.get('paths', {}).items():
-        for method, operation in path.items():
-            method_markdown = ''
-            summary = operation.get('summary', '*no summary*')
-            method_markdown += f"### {summary}\n\n"
-            description = operation.get('description', '*no description*')
-            method_markdown += f"{description}\n\n"
-            method_markdown += f"**route:** `{route}`\n\n"
-            method_markdown += f"**method:** `{method.upper()}`\n\n"
-            tag = operation.get('tags', ['default'])[0]
-            parameters = operation.get('parameters', [])
-            if parameters:
-                method_markdown += "**parameters:** \n\n"
-                method_markdown += parse_parameters(parameters)
-            request_body = operation.get('requestBody')
-            if request_body:
-                method_markdown += "**requestBody:** \n\n"
-                method_markdown += parse_request_body(request_body, schemas_dict)
-            tag_dict[tag]['paths'] += f"{method_markdown}\n\n"
-
-    for tag, value in tag_dict.items():
-        paths = value.get('paths', '')
-        if paths:
-            markdown += f"## {tag}\n\n"
-            markdown += f"{value.get('description', '*no description*')}\n\n"
-            markdown += f"{paths}\n"
-    if schemas:
-        markdown += "## schemas\n\n"
-        for name, obj in schemas_dict.items():
-            markdown += f"### {name}\n\n"
-            markdown += f"{obj}\n\n"
-
-    return markdown
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/8/11 10:39
+from .models import OPENAPI3_REF_PREFIX
+
+
+def parse_schemas(schemas):
+    schemas_dict = {}
+    for name, obj in schemas.items():
+        schemas_dict[name] = "| name | type | required | description |\n"
+        schemas_dict[name] += "| ---- | ---- | -------- | ----------- |\n"
+        required = obj.get('required', [])
+        enum = obj.get('enum')
+        if enum:
+            schemas_dict[name] += f"| {name} | {obj.get('type', '')} | - | Enum: {', '.join(enum)} |\n"
+        properties = obj.get('properties')
+        if properties:
+            for property_name, _property in properties.items():
+                ref = _property.get('$ref')
+                if ref:
+                    ref_name = ref.lstrip(OPENAPI3_REF_PREFIX + '/')
+                    schemas_dict[name] += f"| {property_name} | - | - | [{ref_name}](#{ref_name}) |\n"
+                else:
+                    schemas_dict[name] += f"| {property_name} " \
+                                          f"| {_property.get('format', '') or _property.get('type', '')} " \
+                                          f"| {property_name in required} " \
+                                          f"| {_property.get('description', '')} " \
+                                          f"|\n"
+    return schemas_dict
+
+
+def parse_parameters(parameters):
+    md = "| name | type | in   | required | description |\n"
+    md += "| ---- | ---- | ---- | -------- | ----------- |\n"
+    for param in parameters:
+        aff_of = param['schema'].get('allOf')
+        if aff_of:
+            for one in aff_of:
+                if isinstance(one, dict) and one.get('$ref'):
+                    ref_name = one.get('$ref').lstrip(OPENAPI3_REF_PREFIX + '/')
+                    md += f"| {param.get('name', '')} " \
+                          f"| {param['schema'].get('type', '')} " \
+                          f"| {param.get('in', '')} " \
+                          f"| {param.get('required', '')} " \
+                          f"| [{ref_name}](#{ref_name}) " \
+                          f"|\n"
+                    break
+            continue
+        md += f"| {param.get('name', '')} " \
+              f"| {param['schema'].get('type', '')} " \
+              f"| {param.get('in', '')} " \
+              f"| {param.get('required', '')} " \
+              f"| {param.get('description', '')} " \
+              f"|\n"
+    md += "\n"
+    return md
+
+
+def parse_request_body(request_body, schemas_dict):
+    md = ''
+    content = request_body['content']
+    for media_type, schemas in content.items():
+        md += f"*{media_type}*\n\n"
+        ref = schemas['schema']['$ref']
+        obj_name = ref.lstrip(OPENAPI3_REF_PREFIX + '/')
+        md += f"{schemas_dict.get(obj_name, '')}"
+    md += "\n"
+    return md
+
+
+def openapi_to_markdown(api_json: dict) -> str:
+    markdown = ''
+    # info and version
+    info = api_json['info']
+    markdown += f"# {info['title']}\n\n"
+    markdown += f"**version**: *{info['version']}*\n\n"
+    # tags
+    tag_dict = {}
+    for tag in api_json.get('tags', []):
+        tag_dict[tag['name']] = {'description': tag['description'], 'paths': ''}
+    if not tag_dict.get('default'):
+        tag_dict['default'] = {'paths': ''}
+    # schemas
+    components = api_json.get("components", {})
+    schemas = components.get('schemas', {})
+    schemas_dict = parse_schemas(schemas)
+    # paths
+    for route, path in api_json.get('paths', {}).items():
+        for method, operation in path.items():
+            method_markdown = ''
+            summary = operation.get('summary', '*no summary*')
+            method_markdown += f"### {summary}\n\n"
+            description = operation.get('description', '*no description*')
+            method_markdown += f"{description}\n\n"
+            method_markdown += f"**route:** `{route}`\n\n"
+            method_markdown += f"**method:** `{method.upper()}`\n\n"
+            tag = operation.get('tags', ['default'])[0]
+            parameters = operation.get('parameters', [])
+            if parameters:
+                method_markdown += "**parameters:** \n\n"
+                method_markdown += parse_parameters(parameters)
+            request_body = operation.get('requestBody')
+            if request_body:
+                method_markdown += "**requestBody:** \n\n"
+                method_markdown += parse_request_body(request_body, schemas_dict)
+            tag_dict[tag]['paths'] += f"{method_markdown}\n\n"
+
+    for tag, value in tag_dict.items():
+        paths = value.get('paths', '')
+        if paths:
+            markdown += f"## {tag}\n\n"
+            markdown += f"{value.get('description', '*no description*')}\n\n"
+            markdown += f"{paths}\n"
+    if schemas:
+        markdown += "## schemas\n\n"
+        for name, obj in schemas_dict.items():
+            markdown += f"### {name}\n\n"
+            markdown += f"{obj}\n\n"
+
+    return markdown
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/request.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/request.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/4/1 16:54
-import json
-from json import JSONDecodeError
-from typing import Any, Type, Optional, Dict, Union
-
-from flask import request, current_app, abort
-from pydantic import ValidationError, BaseModel
-
-
-def _validate_header(header: Type[BaseModel], func_kwargs):
-    request_headers = dict(request.headers) or {}
-    for key, value in header.model_json_schema().get("properties", {}).items():
-        key_title = key.replace("_", "-").title()
-        # Add original key
-        if key_title in request_headers.keys():
-            request_headers[key] = request_headers[key_title]
-    func_kwargs.update({"header": header.model_validate(obj=request_headers)})
-
-
-def _validate_cookie(cookie: Type[BaseModel], func_kwargs):
-    request_cookies = dict(request.cookies) or {}
-    func_kwargs.update({"cookie": cookie.model_validate(obj=request_cookies)})
-
-
-def _validate_path(path: Type[BaseModel], path_kwargs, func_kwargs):
-    func_kwargs.update({"path": path.model_validate(obj=path_kwargs)})
-
-
-def _validate_query(query: Type[BaseModel], func_kwargs):
-    request_args = request.args
-    query_dict = {}
-    for k, v in query.model_json_schema().get("properties", {}).items():
-        value: Union[list, Optional[str]]
-        if v.get("type") == "array":
-            value = request_args.getlist(k)
-        else:
-            value = request_args.get(k)
-        if value is not None:
-            query_dict[k] = value
-    func_kwargs.update({"query": query.model_validate(obj=query_dict)})
-
-
-def _validate_form(form: Type[BaseModel], func_kwargs):
-    request_form = request.form
-    request_files = request.files
-    form_dict = {}
-    for k, v in form.model_json_schema().get("properties", {}).items():
-        if v.get("type") == "array":
-            items = v.get("items", {})
-            if items.get("type") == "string" and items.get("format") == "binary":
-                # List[FileStorage]
-                value = request_files.getlist(k)
-            elif items.get("type") in ["object", "null", None]:
-                # list object, None, $ref, anyOf
-                value = []
-                for i in request_form.getlist(k):
-                    try:
-                        json_loads_result = json.loads(i)
-                    except JSONDecodeError:
-                        json_loads_result = i
-                    value.append(json_loads_result)
-            else:
-                # List[str], List[int] ...
-                value = request_form.getlist(k)  # type:ignore
-        elif v.get("type") in ["object", "null", None]:
-            # list object, None, $ref, anyOf
-            try:
-                value = json.loads(request_form.get(k)) if request_form.get(k) else None  # type:ignore
-            except JSONDecodeError:
-                value = request_form.get(k)  # type:ignore
-        else:
-            if v.get("format") == "binary":
-                # FileStorage
-                value = request_files.get(k)  # type:ignore
-            else:
-                # str, int ...
-                value = request_form.get(k)  # type:ignore
-        if value is not None:
-            form_dict[k] = value
-    func_kwargs.update({"form": form.model_validate(obj=form_dict)})
-
-
-def _validate_body(body: Type[BaseModel], func_kwargs):
-    obj = request.get_json(silent=True) or {}
-    if isinstance(obj, str):
-        body_model = body.model_validate_json(json_data=obj)
-    else:
-        body_model = body.model_validate(obj=obj)
-    func_kwargs.update({"body": body_model})
-
-
-def _validate_request(
-        header: Optional[Type[BaseModel]] = None,
-        cookie: Optional[Type[BaseModel]] = None,
-        path: Optional[Type[BaseModel]] = None,
-        query: Optional[Type[BaseModel]] = None,
-        form: Optional[Type[BaseModel]] = None,
-        body: Optional[Type[BaseModel]] = None,
-        raw: Optional[Type[BaseModel]] = None,
-        path_kwargs: Optional[Dict[Any, Any]] = None
-) -> Dict:
-    """
-    Validate requests and responses.
-
-    Args:
-        header: Header model.
-        cookie: Cookie model.
-        path: Path model.
-        query: Query model.
-        form: Form model.
-        body: Body model.
-        path_kwargs: Path parameters.
-
-    Returns:
-        Union[Response, Dict]: Request kwargs.
-
-    Raises:
-        ValidationError: If validation fails.
-    """
-
-    # Dictionary to store func kwargs
-    func_kwargs: Dict = dict()
-
-    try:
-        # Validate header, cookie, path, and query parameters
-        if header:
-            _validate_header(header, func_kwargs)
-        if cookie:
-            _validate_cookie(cookie, func_kwargs)
-        if path:
-            _validate_path(path, path_kwargs, func_kwargs)
-        if query:
-            _validate_query(query, func_kwargs)
-        if form:
-            _validate_form(form, func_kwargs)
-        if body:
-            _validate_body(body, func_kwargs)
-        if raw:
-            func_kwargs.update({"raw": request})
-    except ValidationError as e:
-        # Create a response with validation error details
-        validation_error_callback = getattr(current_app, "validation_error_callback")
-        abort(validation_error_callback(e))
-
-    return func_kwargs
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/4/1 16:54
+import json
+from json import JSONDecodeError
+from typing import Any, Type, Optional, Dict, Union
+
+from flask import request, current_app, abort
+from pydantic import ValidationError, BaseModel
+
+
+def _validate_header(header: Type[BaseModel], func_kwargs):
+    request_headers = dict(request.headers) or {}
+    for key, value in header.model_json_schema().get("properties", {}).items():
+        key_title = key.replace("_", "-").title()
+        # Add original key
+        if key_title in request_headers.keys():
+            request_headers[key] = request_headers[key_title]
+    func_kwargs.update({"header": header.model_validate(obj=request_headers)})
+
+
+def _validate_cookie(cookie: Type[BaseModel], func_kwargs):
+    request_cookies = dict(request.cookies) or {}
+    func_kwargs.update({"cookie": cookie.model_validate(obj=request_cookies)})
+
+
+def _validate_path(path: Type[BaseModel], path_kwargs, func_kwargs):
+    func_kwargs.update({"path": path.model_validate(obj=path_kwargs)})
+
+
+def _validate_query(query: Type[BaseModel], func_kwargs):
+    request_args = request.args
+    query_dict = {}
+    for k, v in query.model_json_schema().get("properties", {}).items():
+        value: Union[list, Optional[str]]
+        if v.get("type") == "array":
+            value = request_args.getlist(k)
+        else:
+            value = request_args.get(k)
+        if value is not None:
+            query_dict[k] = value
+    func_kwargs.update({"query": query.model_validate(obj=query_dict)})
+
+
+def _validate_form(form: Type[BaseModel], func_kwargs):
+    request_form = request.form
+    request_files = request.files
+    form_dict = {}
+    for k, v in form.model_json_schema().get("properties", {}).items():
+        if v.get("type") == "array":
+            items = v.get("items", {})
+            if items.get("type") == "string" and items.get("format") == "binary":
+                # List[FileStorage]
+                value = request_files.getlist(k)
+            elif items.get("type") in ["object", "null", None]:
+                # list object, None, $ref, anyOf
+                value = []
+                for i in request_form.getlist(k):
+                    try:
+                        json_loads_result = json.loads(i)
+                    except JSONDecodeError:
+                        json_loads_result = i
+                    value.append(json_loads_result)
+            else:
+                # List[str], List[int] ...
+                value = request_form.getlist(k)  # type:ignore
+        elif v.get("type") in ["object", "null", None]:
+            # list object, None, $ref, anyOf
+            try:
+                value = json.loads(request_form.get(k)) if request_form.get(k) else None  # type:ignore
+            except JSONDecodeError:
+                value = request_form.get(k)  # type:ignore
+        else:
+            if v.get("format") == "binary":
+                # FileStorage
+                value = request_files.get(k)  # type:ignore
+            else:
+                # str, int ...
+                value = request_form.get(k)  # type:ignore
+        if value is not None:
+            form_dict[k] = value
+    func_kwargs.update({"form": form.model_validate(obj=form_dict)})
+
+
+def _validate_body(body: Type[BaseModel], func_kwargs):
+    obj = request.get_json(silent=True) or {}
+    if isinstance(obj, str):
+        body_model = body.model_validate_json(json_data=obj)
+    else:
+        body_model = body.model_validate(obj=obj)
+    func_kwargs.update({"body": body_model})
+
+
+def _validate_request(
+        header: Optional[Type[BaseModel]] = None,
+        cookie: Optional[Type[BaseModel]] = None,
+        path: Optional[Type[BaseModel]] = None,
+        query: Optional[Type[BaseModel]] = None,
+        form: Optional[Type[BaseModel]] = None,
+        body: Optional[Type[BaseModel]] = None,
+        raw: Optional[Type[BaseModel]] = None,
+        path_kwargs: Optional[Dict[Any, Any]] = None
+) -> Dict:
+    """
+    Validate requests and responses.
+
+    Args:
+        header: Header model.
+        cookie: Cookie model.
+        path: Path model.
+        query: Query model.
+        form: Form model.
+        body: Body model.
+        path_kwargs: Path parameters.
+
+    Returns:
+        Union[Response, Dict]: Request kwargs.
+
+    Raises:
+        ValidationError: If validation fails.
+    """
+
+    # Dictionary to store func kwargs
+    func_kwargs: Dict = dict()
+
+    try:
+        # Validate header, cookie, path, and query parameters
+        if header:
+            _validate_header(header, func_kwargs)
+        if cookie:
+            _validate_cookie(cookie, func_kwargs)
+        if path:
+            _validate_path(path, path_kwargs, func_kwargs)
+        if query:
+            _validate_query(query, func_kwargs)
+        if form:
+            _validate_form(form, func_kwargs)
+        if body:
+            _validate_body(body, func_kwargs)
+        if raw:
+            func_kwargs.update({"raw": request})
+    except ValidationError as e:
+        # Create a response with validation error details
+        validation_error_callback = getattr(current_app, "validation_error_callback")
+        abort(validation_error_callback(e))
+
+    return func_kwargs
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/scaffold.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/scaffold.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,438 +1,438 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/8/30 9:40
-import inspect
-from functools import wraps
-from typing import Callable, List, Optional, Dict, Any
-
-from flask.wrappers import Response as FlaskResponse
-
-from .models import ExternalDocumentation
-from .models import Server
-from .models import Tag
-from .request import _validate_request
-from .types import ParametersTuple
-from .types import ResponseDict
-from .utils import HTTPMethod
-
-
-class APIScaffold:
-    def _collect_openapi_info(
-            self,
-            rule: str,
-            func: Callable,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True,
-            method: str = HTTPMethod.GET
-    ) -> ParametersTuple:
-        raise NotImplementedError
-
-    def register_api(self, api) -> None:
-        raise NotImplementedError
-
-    def _add_url_rule(
-            self,
-            rule,
-            endpoint=None,
-            view_func=None,
-            provide_automatic_options=None,
-            **options,
-    ) -> None:
-        raise NotImplementedError
-
-    @staticmethod
-    def create_view_func(
-            func,
-            header,
-            cookie,
-            path,
-            query,
-            form,
-            body,
-            raw,
-            view_class=None,
-            view_kwargs=None
-    ):
-        is_coroutine_function = inspect.iscoroutinefunction(func)
-        if is_coroutine_function:
-            @wraps(func)
-            async def view_func(**kwargs) -> FlaskResponse:
-                func_kwargs = _validate_request(
-                    header=header,
-                    cookie=cookie,
-                    path=path,
-                    query=query,
-                    form=form,
-                    body=body,
-                    raw=raw,
-                    path_kwargs=kwargs
-                )
-
-                # handle async request
-                if view_class:
-                    signature = inspect.signature(view_class.__init__)
-                    parameters = signature.parameters
-                    if parameters.get("view_kwargs"):
-                        view_object = view_class(view_kwargs=view_kwargs)
-                    else:
-                        view_object = view_class()
-                    response = await func(view_object, **func_kwargs)
-                else:
-                    response = await func(**func_kwargs)
-                return response
-        else:
-            @wraps(func)
-            def view_func(**kwargs) -> FlaskResponse:
-                func_kwargs = _validate_request(
-                    header=header,
-                    cookie=cookie,
-                    path=path,
-                    query=query,
-                    form=form,
-                    body=body,
-                    raw=raw,
-                    path_kwargs=kwargs
-                )
-
-                # handle request
-                if view_class:
-                    signature = inspect.signature(view_class.__init__)
-                    parameters = signature.parameters
-                    if parameters.get("view_kwargs"):
-                        view_object = view_class(view_kwargs=view_kwargs)
-                    else:
-                        view_object = view_class()
-                    response = func(view_object, **func_kwargs)
-                else:
-                    response = func(**func_kwargs)
-                return response
-
-        if not hasattr(func, "view"):
-            func.view = view_func
-
-        return func.view
-
-    def get(
-            self,
-            rule: str,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True,
-            **options: Any
-    ) -> Callable:
-        """
-        Decorator for defining a REST API endpoint with the HTTP GET method.
-        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
-
-        Args:
-            rule: The URL rule string.
-            tags: Adds metadata to a single tag.
-            summary: A short summary of what the operation does.
-            description: A verbose explanation of the operation behavior.
-            external_docs: Additional external documentation for this operation.
-            operation_id: Unique string used to identify the operation.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            deprecated: Declares this operation to be deprecated.
-            security: A declaration of which security mechanisms can be used for this operation.
-            servers: An alternative server array to service this operation.
-            openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown. Default to True.
-        """
-
-        def decorator(func) -> Callable:
-            header, cookie, path, query, form, body, raw = \
-                self._collect_openapi_info(
-                    rule,
-                    func,
-                    tags=tags,
-                    summary=summary,
-                    description=description,
-                    external_docs=external_docs,
-                    operation_id=operation_id,
-                    responses=responses,
-                    deprecated=deprecated,
-                    security=security,
-                    servers=servers,
-                    openapi_extensions=openapi_extensions,
-                    doc_ui=doc_ui,
-                    method=HTTPMethod.GET
-                )
-
-            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
-            options.update({"methods": [HTTPMethod.GET]})
-            self._add_url_rule(rule, view_func=view_func, **options)
-
-            return func
-
-        return decorator
-
-    def post(
-            self,
-            rule: str,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True,
-            **options: Any
-    ) -> Callable:
-        """
-        Decorator for defining a REST API endpoint with the HTTP POST method.
-        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
-
-        Args:
-            rule: The URL rule string.
-            tags: Adds metadata to a single tag.
-            summary: A short summary of what the operation does.
-            description: A verbose explanation of the operation behavior.
-            external_docs: Additional external documentation for this operation.
-            operation_id: Unique string used to identify the operation.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            deprecated: Declares this operation to be deprecated.
-            security: A declaration of which security mechanisms can be used for this operation.
-            servers: An alternative server array to service this operation.
-            openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown. Default to True.
-        """
-
-        def decorator(func) -> Callable:
-            header, cookie, path, query, form, body, raw = \
-                self._collect_openapi_info(
-                    rule,
-                    func,
-                    tags=tags,
-                    summary=summary,
-                    description=description,
-                    external_docs=external_docs,
-                    operation_id=operation_id,
-                    responses=responses,
-                    deprecated=deprecated,
-                    security=security,
-                    servers=servers,
-                    openapi_extensions=openapi_extensions,
-                    doc_ui=doc_ui,
-                    method=HTTPMethod.POST
-                )
-
-            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
-            options.update({"methods": [HTTPMethod.POST]})
-            self._add_url_rule(rule, view_func=view_func, **options)
-
-            return func
-
-        return decorator
-
-    def put(
-            self,
-            rule: str,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True,
-            **options: Any
-    ) -> Callable:
-        """
-        Decorator for defining a REST API endpoint with the HTTP PUT method.
-        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
-
-        Args:
-            rule: The URL rule string.
-            tags: Adds metadata to a single tag.
-            summary: A short summary of what the operation does.
-            description: A verbose explanation of the operation behavior.
-            external_docs: Additional external documentation for this operation.
-            operation_id: Unique string used to identify the operation.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            deprecated: Declares this operation to be deprecated.
-            security: A declaration of which security mechanisms can be used for this operation.
-            servers: An alternative server array to service this operation.
-            openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown. Default to True.
-        """
-
-        def decorator(func) -> Callable:
-            header, cookie, path, query, form, body, raw = \
-                self._collect_openapi_info(
-                    rule,
-                    func,
-                    tags=tags,
-                    summary=summary,
-                    description=description,
-                    external_docs=external_docs,
-                    operation_id=operation_id,
-                    responses=responses,
-                    deprecated=deprecated,
-                    security=security,
-                    servers=servers,
-                    openapi_extensions=openapi_extensions,
-                    doc_ui=doc_ui,
-                    method=HTTPMethod.PUT
-                )
-
-            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
-            options.update({"methods": [HTTPMethod.PUT]})
-            self._add_url_rule(rule, view_func=view_func, **options)
-
-            return func
-
-        return decorator
-
-    def delete(
-            self,
-            rule: str,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True,
-            **options: Any
-    ) -> Callable:
-        """
-        Decorator for defining a REST API endpoint with the HTTP DELETE method.
-        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
-
-        Args:
-            rule: The URL rule string.
-            tags: Adds metadata to a single tag.
-            summary: A short summary of what the operation does.
-            description: A verbose explanation of the operation behavior.
-            external_docs: Additional external documentation for this operation.
-            operation_id: Unique string used to identify the operation.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            deprecated: Declares this operation to be deprecated.
-            security: A declaration of which security mechanisms can be used for this operation.
-            servers: An alternative server array to service this operation.
-            openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown. Default to True.
-        """
-
-        def decorator(func) -> Callable:
-            header, cookie, path, query, form, body, raw = \
-                self._collect_openapi_info(
-                    rule,
-                    func,
-                    tags=tags,
-                    summary=summary,
-                    description=description,
-                    external_docs=external_docs,
-                    operation_id=operation_id,
-                    responses=responses,
-                    deprecated=deprecated,
-                    security=security,
-                    servers=servers,
-                    openapi_extensions=openapi_extensions,
-                    doc_ui=doc_ui,
-                    method=HTTPMethod.DELETE
-                )
-
-            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
-            options.update({"methods": [HTTPMethod.DELETE]})
-            self._add_url_rule(rule, view_func=view_func, **options)
-
-            return func
-
-        return decorator
-
-    def patch(
-            self,
-            rule: str,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True,
-            **options: Any
-    ) -> Callable:
-        """
-        Decorator for defining a REST API endpoint with the HTTP PATCH method.
-        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
-
-        Args:
-            rule: The URL rule string.
-            tags: Adds metadata to a single tag.
-            summary: A short summary of what the operation does.
-            description: A verbose explanation of the operation behavior.
-            external_docs: Additional external documentation for this operation.
-            operation_id: Unique string used to identify the operation.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            deprecated: Declares this operation to be deprecated.
-            security: A declaration of which security mechanisms can be used for this operation.
-            servers: An alternative server array to service this operation.
-            openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown. Default to True.
-        """
-
-        def decorator(func) -> Callable:
-            header, cookie, path, query, form, body, raw = \
-                self._collect_openapi_info(
-                    rule,
-                    func,
-                    tags=tags,
-                    summary=summary,
-                    description=description,
-                    external_docs=external_docs,
-                    operation_id=operation_id,
-                    responses=responses,
-                    deprecated=deprecated,
-                    security=security,
-                    servers=servers,
-                    openapi_extensions=openapi_extensions,
-                    doc_ui=doc_ui,
-                    method=HTTPMethod.PATCH
-                )
-
-            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
-            options.update({"methods": [HTTPMethod.PATCH]})
-            self._add_url_rule(rule, view_func=view_func, **options)
-
-            return func
-
-        return decorator
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/8/30 9:40
+import inspect
+from functools import wraps
+from typing import Callable, List, Optional, Dict, Any
+
+from flask.wrappers import Response as FlaskResponse
+
+from .models import ExternalDocumentation
+from .models import Server
+from .models import Tag
+from .request import _validate_request
+from .types import ParametersTuple
+from .types import ResponseDict
+from .utils import HTTPMethod
+
+
+class APIScaffold:
+    def _collect_openapi_info(
+            self,
+            rule: str,
+            func: Callable,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            method: str = HTTPMethod.GET
+    ) -> ParametersTuple:
+        raise NotImplementedError
+
+    def register_api(self, api) -> None:
+        raise NotImplementedError
+
+    def _add_url_rule(
+            self,
+            rule,
+            endpoint=None,
+            view_func=None,
+            provide_automatic_options=None,
+            **options,
+    ) -> None:
+        raise NotImplementedError
+
+    @staticmethod
+    def create_view_func(
+            func,
+            header,
+            cookie,
+            path,
+            query,
+            form,
+            body,
+            raw,
+            view_class=None,
+            view_kwargs=None
+    ):
+        is_coroutine_function = inspect.iscoroutinefunction(func)
+        if is_coroutine_function:
+            @wraps(func)
+            async def view_func(**kwargs) -> FlaskResponse:
+                func_kwargs = _validate_request(
+                    header=header,
+                    cookie=cookie,
+                    path=path,
+                    query=query,
+                    form=form,
+                    body=body,
+                    raw=raw,
+                    path_kwargs=kwargs
+                )
+
+                # handle async request
+                if view_class:
+                    signature = inspect.signature(view_class.__init__)
+                    parameters = signature.parameters
+                    if parameters.get("view_kwargs"):
+                        view_object = view_class(view_kwargs=view_kwargs)
+                    else:
+                        view_object = view_class()
+                    response = await func(view_object, **func_kwargs)
+                else:
+                    response = await func(**func_kwargs)
+                return response
+        else:
+            @wraps(func)
+            def view_func(**kwargs) -> FlaskResponse:
+                func_kwargs = _validate_request(
+                    header=header,
+                    cookie=cookie,
+                    path=path,
+                    query=query,
+                    form=form,
+                    body=body,
+                    raw=raw,
+                    path_kwargs=kwargs
+                )
+
+                # handle request
+                if view_class:
+                    signature = inspect.signature(view_class.__init__)
+                    parameters = signature.parameters
+                    if parameters.get("view_kwargs"):
+                        view_object = view_class(view_kwargs=view_kwargs)
+                    else:
+                        view_object = view_class()
+                    response = func(view_object, **func_kwargs)
+                else:
+                    response = func(**func_kwargs)
+                return response
+
+        if not hasattr(func, "view"):
+            func.view = view_func
+
+        return func.view
+
+    def get(
+            self,
+            rule: str,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            **options: Any
+    ) -> Callable:
+        """
+        Decorator for defining a REST API endpoint with the HTTP GET method.
+        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
+
+        Args:
+            rule: The URL rule string.
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Declares this operation to be shown. Default to True.
+        """
+
+        def decorator(func) -> Callable:
+            header, cookie, path, query, form, body, raw = \
+                self._collect_openapi_info(
+                    rule,
+                    func,
+                    tags=tags,
+                    summary=summary,
+                    description=description,
+                    external_docs=external_docs,
+                    operation_id=operation_id,
+                    responses=responses,
+                    deprecated=deprecated,
+                    security=security,
+                    servers=servers,
+                    openapi_extensions=openapi_extensions,
+                    doc_ui=doc_ui,
+                    method=HTTPMethod.GET
+                )
+
+            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
+            options.update({"methods": [HTTPMethod.GET]})
+            self._add_url_rule(rule, view_func=view_func, **options)
+
+            return func
+
+        return decorator
+
+    def post(
+            self,
+            rule: str,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            **options: Any
+    ) -> Callable:
+        """
+        Decorator for defining a REST API endpoint with the HTTP POST method.
+        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
+
+        Args:
+            rule: The URL rule string.
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Declares this operation to be shown. Default to True.
+        """
+
+        def decorator(func) -> Callable:
+            header, cookie, path, query, form, body, raw = \
+                self._collect_openapi_info(
+                    rule,
+                    func,
+                    tags=tags,
+                    summary=summary,
+                    description=description,
+                    external_docs=external_docs,
+                    operation_id=operation_id,
+                    responses=responses,
+                    deprecated=deprecated,
+                    security=security,
+                    servers=servers,
+                    openapi_extensions=openapi_extensions,
+                    doc_ui=doc_ui,
+                    method=HTTPMethod.POST
+                )
+
+            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
+            options.update({"methods": [HTTPMethod.POST]})
+            self._add_url_rule(rule, view_func=view_func, **options)
+
+            return func
+
+        return decorator
+
+    def put(
+            self,
+            rule: str,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            **options: Any
+    ) -> Callable:
+        """
+        Decorator for defining a REST API endpoint with the HTTP PUT method.
+        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
+
+        Args:
+            rule: The URL rule string.
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Declares this operation to be shown. Default to True.
+        """
+
+        def decorator(func) -> Callable:
+            header, cookie, path, query, form, body, raw = \
+                self._collect_openapi_info(
+                    rule,
+                    func,
+                    tags=tags,
+                    summary=summary,
+                    description=description,
+                    external_docs=external_docs,
+                    operation_id=operation_id,
+                    responses=responses,
+                    deprecated=deprecated,
+                    security=security,
+                    servers=servers,
+                    openapi_extensions=openapi_extensions,
+                    doc_ui=doc_ui,
+                    method=HTTPMethod.PUT
+                )
+
+            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
+            options.update({"methods": [HTTPMethod.PUT]})
+            self._add_url_rule(rule, view_func=view_func, **options)
+
+            return func
+
+        return decorator
+
+    def delete(
+            self,
+            rule: str,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            **options: Any
+    ) -> Callable:
+        """
+        Decorator for defining a REST API endpoint with the HTTP DELETE method.
+        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
+
+        Args:
+            rule: The URL rule string.
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Declares this operation to be shown. Default to True.
+        """
+
+        def decorator(func) -> Callable:
+            header, cookie, path, query, form, body, raw = \
+                self._collect_openapi_info(
+                    rule,
+                    func,
+                    tags=tags,
+                    summary=summary,
+                    description=description,
+                    external_docs=external_docs,
+                    operation_id=operation_id,
+                    responses=responses,
+                    deprecated=deprecated,
+                    security=security,
+                    servers=servers,
+                    openapi_extensions=openapi_extensions,
+                    doc_ui=doc_ui,
+                    method=HTTPMethod.DELETE
+                )
+
+            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
+            options.update({"methods": [HTTPMethod.DELETE]})
+            self._add_url_rule(rule, view_func=view_func, **options)
+
+            return func
+
+        return decorator
+
+    def patch(
+            self,
+            rule: str,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            **options: Any
+    ) -> Callable:
+        """
+        Decorator for defining a REST API endpoint with the HTTP PATCH method.
+        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
+
+        Args:
+            rule: The URL rule string.
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Declares this operation to be shown. Default to True.
+        """
+
+        def decorator(func) -> Callable:
+            header, cookie, path, query, form, body, raw = \
+                self._collect_openapi_info(
+                    rule,
+                    func,
+                    tags=tags,
+                    summary=summary,
+                    description=description,
+                    external_docs=external_docs,
+                    operation_id=operation_id,
+                    responses=responses,
+                    deprecated=deprecated,
+                    security=security,
+                    servers=servers,
+                    openapi_extensions=openapi_extensions,
+                    doc_ui=doc_ui,
+                    method=HTTPMethod.PATCH
+                )
+
+            view_func = self.create_view_func(func, header, cookie, path, query, form, body, raw)
+            options.update({"methods": [HTTPMethod.PATCH]})
+            self._add_url_rule(rule, view_func=view_func, **options)
+
+            return func
+
+        return decorator
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/types.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/types.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/9 15:25
-from http import HTTPStatus
-from typing import Dict, Union, Type, Any, Tuple, Optional
-
-from pydantic import BaseModel
-
-from .models import RawModel
-from .models import SecurityScheme
-
-_ResponseDictValue = Union[Type[BaseModel], Dict[Any, Any], None]
-
-ResponseDict = Dict[Union[str, int, HTTPStatus], _ResponseDictValue]
-
-ResponseStrKeyDict = Dict[str, _ResponseDictValue]
-
-SecuritySchemesDict = Dict[str, Union[SecurityScheme, Dict[str, Any]]]
-
-ParametersTuple = Tuple[
-    Optional[Type[BaseModel]],
-    Optional[Type[BaseModel]],
-    Optional[Type[BaseModel]],
-    Optional[Type[BaseModel]],
-    Optional[Type[BaseModel]],
-    Optional[Type[BaseModel]],
-    Optional[Type[RawModel]]
-]
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/9 15:25
+from http import HTTPStatus
+from typing import Dict, Union, Type, Any, Tuple, Optional
+
+from pydantic import BaseModel
+
+from .models import RawModel
+from .models import SecurityScheme
+
+_ResponseDictValue = Union[Type[BaseModel], Dict[Any, Any], None]
+
+ResponseDict = Dict[Union[str, int, HTTPStatus], _ResponseDictValue]
+
+ResponseStrKeyDict = Dict[str, _ResponseDictValue]
+
+SecuritySchemesDict = Dict[str, Union[SecurityScheme, Dict[str, Any]]]
+
+ParametersTuple = Tuple[
+    Optional[Type[BaseModel]],
+    Optional[Type[BaseModel]],
+    Optional[Type[BaseModel]],
+    Optional[Type[BaseModel]],
+    Optional[Type[BaseModel]],
+    Optional[Type[BaseModel]],
+    Optional[Type[RawModel]]
+]
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/utils.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,596 +1,596 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/5/1 21:34
-
-import inspect
-import re
-import sys
-from enum import Enum
-from http import HTTPStatus
-from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional, Any, DefaultDict
-
-from flask import make_response, current_app
-from flask.wrappers import Response as FlaskResponse
-from pydantic import BaseModel, ValidationError
-from pydantic.json_schema import JsonSchemaMode
-
-from .models import Encoding
-from .models import MediaType
-from .models import OPENAPI3_REF_PREFIX
-from .models import OPENAPI3_REF_TEMPLATE
-from .models import Operation
-from .models import Parameter
-from .models import ParameterInType
-from .models import PathItem
-from .models import RawModel
-from .models import RequestBody
-from .models import Response
-from .models import Schema
-from .models import Tag
-from .models.data_type import DataType
-from .types import ParametersTuple
-from .types import ResponseDict
-from .types import ResponseStrKeyDict
-
-HTTP_STATUS = {str(status.value): status.phrase for status in HTTPStatus}
-
-if sys.version_info < (3, 11):
-
-    class HTTPMethod(str, Enum):
-        GET = "GET"
-        POST = "POST"
-        PUT = "PUT"
-        DELETE = "DELETE"
-        PATCH = "PATCH"
-        HEAD = "HEAD"
-        OPTIONS = "OPTIONS"
-        TRACE = "TRACE"
-        CONNECT = "CONNECT"
-else:
-    from http import HTTPMethod
-
-
-def get_operation(
-        func: Callable, *,
-        summary: Optional[str] = None,
-        description: Optional[str] = None,
-        openapi_extensions: Optional[Dict[str, Any]] = None,
-) -> Operation:
-    """
-    Return an Operation object with the specified summary and description.
-
-    Args:
-        func: The function or method for which the operation is being defined.
-        summary: A short summary of what the operation does.
-        description: A verbose explanation of the operation behavior.
-        openapi_extensions: Additional extensions to the OpenAPI Schema.
-
-    Returns:
-        An Operation object representing the operation.
-
-    """
-    # Get the docstring of the function
-    doc = inspect.getdoc(func) or ""
-    doc = doc.strip()
-    lines = doc.split("\n")
-    doc_summary = lines[0] or None
-
-    # Determine the summary and description based on provided arguments or docstring
-    if summary is None:
-        doc_description = lines[0] if len(lines) == 0 else "</br>".join(lines[1:]) or None
-    else:
-        doc_description = "</br>".join(lines) or None
-
-    # Create the operation dictionary with summary and description
-    operation_dict = dict(
-        summary=summary or doc_summary,
-        description=description or doc_description
-    )
-
-    # Add any additional openapi_extensions to the operation dictionary
-    openapi_extensions = openapi_extensions or {}
-    operation_dict.update(**openapi_extensions)
-
-    # Create and return the Operation object
-    operation = Operation(**operation_dict)
-
-    return operation
-
-
-def get_operation_id_for_path(*, name: str, path: str, method: str) -> str:
-    """
-    Generate a unique operation ID based on the name, path, and method.
-
-    Args:
-        name: The name or identifier for the operation.
-        path: The URL path for the operation.
-        method: The HTTP method for the operation.
-
-    Returns:
-        A unique operation ID generated based on the provided name, path, and method.
-
-    """
-    operation_id = name + path
-    # Replace non-word characters with underscores
-    operation_id = re.sub(r"\W", "_", operation_id)
-    operation_id = operation_id + "_" + method.lower()
-    return operation_id
-
-
-def get_model_schema(model: Type[BaseModel], mode: JsonSchemaMode = "validation") -> dict:
-    """Converts a Pydantic model to an OpenAPI schema."""
-
-    assert inspect.isclass(model) and issubclass(model, BaseModel), \
-        f"{model} is invalid `pydantic.BaseModel`"
-
-    model_config = model.model_config
-    by_alias = bool(model_config.get("by_alias", True))
-
-    return model.model_json_schema(by_alias=by_alias, ref_template=OPENAPI3_REF_TEMPLATE, mode=mode)
-
-
-def parse_header(header: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a header model and returns a list of parameters and component schemas."""
-    schema = get_model_schema(header)
-    parameters = []
-    components_schemas: Dict = dict()
-    properties = schema.get("properties", {})
-
-    for name, value in properties.items():
-        data = {
-            "name": name,
-            "in": ParameterInType.HEADER,
-            "description": value.get("description"),
-            "required": name in schema.get("required", []),
-            "schema": Schema(**value)
-        }
-        # Parse extra values
-        data.update({
-            "deprecated": value.get("deprecated"),
-            "example": value.get("example"),
-            "examples": value.get("examples"),
-        })
-        parameters.append(Parameter(**data))
-
-    # Parse definitions
-    definitions = schema.get("$defs", {})
-    for name, value in definitions.items():
-        components_schemas[name] = Schema(**value)
-
-    return parameters, components_schemas
-
-
-def parse_cookie(cookie: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a cookie model and returns a list of parameters and component schemas."""
-    schema = get_model_schema(cookie)
-    parameters = []
-    components_schemas: Dict = dict()
-    properties = schema.get("properties", {})
-
-    for name, value in properties.items():
-        data = {
-            "name": name,
-            "in": ParameterInType.COOKIE,
-            "description": value.get("description"),
-            "required": name in schema.get("required", []),
-            "schema": Schema(**value)
-        }
-        # Parse extra values
-        data.update({
-            "deprecated": value.get("deprecated"),
-            "example": value.get("example"),
-            "examples": value.get("examples"),
-        })
-        parameters.append(Parameter(**data))
-
-    # Parse definitions
-    definitions = schema.get("$defs", {})
-    for name, value in definitions.items():
-        components_schemas[name] = Schema(**value)
-
-    return parameters, components_schemas
-
-
-def parse_path(path: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a path model and returns a list of parameters and component schemas."""
-    schema = get_model_schema(path)
-    parameters = []
-    components_schemas: Dict = dict()
-    properties = schema.get("properties", {})
-
-    for name, value in properties.items():
-        data = {
-            "name": name,
-            "in": ParameterInType.PATH,
-            "description": value.get("description"),
-            "required": True,
-            "schema": Schema(**value)
-        }
-        # Parse extra values
-        data.update({
-            "deprecated": value.get("deprecated"),
-            "example": value.get("example"),
-            "examples": value.get("examples"),
-        })
-        parameters.append(Parameter(**data))
-
-    # Parse definitions
-    definitions = schema.get("$defs", {})
-    for name, value in definitions.items():
-        components_schemas[name] = Schema(**value)
-
-    return parameters, components_schemas
-
-
-def parse_query(query: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
-    """Parses a query model and returns a list of parameters and component schemas."""
-    schema = get_model_schema(query)
-    parameters = []
-    components_schemas: Dict = dict()
-    properties = schema.get("properties", {})
-
-    for name, value in properties.items():
-        data = {
-            "name": name,
-            "in": ParameterInType.QUERY,
-            "description": value.get("description"),
-            "required": name in schema.get("required", []),
-            "schema": Schema(**value)
-        }
-        # Parse extra values
-        data.update({
-            "deprecated": value.get("deprecated"),
-            "example": value.get("example"),
-            "examples": value.get("examples"),
-        })
-        parameters.append(Parameter(**data))
-
-    # Parse definitions
-    definitions = schema.get("$defs", {})
-    for name, value in definitions.items():
-        components_schemas[name] = Schema(**value)
-
-    return parameters, components_schemas
-
-
-def parse_form(
-        form: Type[BaseModel],
-) -> Tuple[Dict[str, MediaType], dict]:
-    """Parses a form model and returns a list of parameters and component schemas."""
-    schema = get_model_schema(form)
-    components_schemas = dict()
-    properties = schema.get("properties", {})
-
-    assert properties, f"{form.__name__}'s properties cannot be empty."
-
-    original_title = schema.get("title") or form.__name__
-    title = normalize_name(original_title)
-    components_schemas[title] = Schema(**schema)
-    encoding = {}
-    for k, v in properties.items():
-        if v.get("type") == "array":
-            encoding[k] = Encoding(style="form", explode=True)
-    content = {
-        "multipart/form-data": MediaType(
-            schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
-            encoding=encoding or None
-        )
-    }
-
-    # Parse definitions
-    definitions = schema.get("$defs", {})
-    for name, value in definitions.items():
-        components_schemas[name] = Schema(**value)
-
-    return content, components_schemas
-
-
-def parse_body(
-        body: Type[BaseModel],
-) -> Tuple[Dict[str, MediaType], dict]:
-    """Parses a body model and returns a list of parameters and component schemas."""
-    schema = get_model_schema(body)
-    components_schemas = dict()
-
-    original_title = schema.get("title") or body.__name__
-    title = normalize_name(original_title)
-    components_schemas[title] = Schema(**schema)
-    content = {
-        "application/json": MediaType(
-            schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"})
-        )
-    }
-
-    # Parse definitions
-    definitions = schema.get("$defs", {})
-    for name, value in definitions.items():
-        components_schemas[name] = Schema(**value)
-
-    return content, components_schemas
-
-
-def get_responses(
-        responses: ResponseStrKeyDict,
-        components_schemas: dict,
-        operation: Operation
-) -> None:
-    _responses = {}
-    _schemas = {}
-
-    for key, response in responses.items():
-        if response is None:
-            # If the response is None, it means HTTP status code "204" (No Content)
-            _responses[key] = Response(description=HTTP_STATUS.get(key, ""))
-        elif isinstance(response, dict):
-            if not response.get("description"):
-                response["description"] = HTTP_STATUS.get(key, "")
-            _responses[key] = Response(**response)
-        else:
-            # OpenAPI 3 support ^[a-zA-Z0-9\.\-_]+$ so we should normalize __name__
-            name = normalize_name(response.__name__)
-            schema = get_model_schema(response, mode="serialization")
-            _responses[key] = Response(
-                description=HTTP_STATUS.get(key, ""),
-                content={
-                    "application/json": MediaType(
-                        schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{name}"})
-                    )})
-
-            model_config: DefaultDict[str, Any] = response.model_config  # type: ignore
-            openapi_extra = model_config.get("openapi_extra")
-            if openapi_extra:
-                # Add additional information from model_config to the response
-                _responses[key].description = openapi_extra.get("description")
-                _responses[key].headers = openapi_extra.get("headers")
-                _responses[key].links = openapi_extra.get("links")
-                _content = _responses[key].content
-                if _content is not None:
-                    _content["application/json"].example = openapi_extra.get("example")
-                    _content["application/json"].examples = openapi_extra.get("examples")
-                    _content["application/json"].encoding = openapi_extra.get("encoding")
-                    _content.update(openapi_extra.get("content", {}))
-
-            _schemas[name] = Schema(**schema)
-            definitions = schema.get("$defs")
-            if definitions:
-                # Add schema definitions to _schemas
-                for name, value in definitions.items():
-                    _schemas[normalize_name(name)] = Schema(**value)
-
-    components_schemas.update(**_schemas)
-    operation.responses = _responses
-
-
-def parse_and_store_tags(
-        new_tags: List[Tag],
-        old_tags: List[Tag],
-        old_tag_names: List[str],
-        operation: Operation
-) -> None:
-    """
-    Parses new tags, stores them in an old_tags list if they are not already present,
-    and updates the tags attribute of the operation object.
-
-    Args:
-        new_tags: A list of new Tag objects to be parsed and stored.
-        old_tags: The list of existing Tag objects.
-        old_tag_names: The list that names of existing tags.
-        operation: The operation object whose tag attribute needs to be updated.
-
-    Returns:
-        None
-    """
-    # Iterate over each tag in new_tags
-    for tag in new_tags:
-        if tag.name not in old_tag_names:
-            old_tag_names.append(tag.name)
-            old_tags.append(tag)
-
-    # Set the tags attribute of the operation object to a list of unique tag names from new_tags
-    # If the resulting list is empty, set it to None
-    operation.tags = list(set([tag.name for tag in new_tags])) or None
-
-
-def parse_parameters(
-        func: Callable,
-        *,
-        components_schemas: Optional[Dict] = None,
-        operation: Optional[Operation] = None,
-        doc_ui: bool = True,
-) -> ParametersTuple:
-    """
-    Parses the parameters of a given function and returns the types for header, cookie, path,
-    query, form, and body parameters. Also populates the Operation object with the parsed parameters.
-
-    Args:
-        func: The function to parse the parameters from.
-        components_schemas: Dictionary to store the parsed components schemas (default: None).
-        operation: Operation object to populate with parsed parameters (default: None).
-        doc_ui: Flag indicating whether to return types for documentation UI (default: True).
-
-    Returns:
-        Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
-        The types for header, cookie, path, query, form, and body parameters respectively.
-
-    """
-    # Get the type hints from the function
-    annotations = get_type_hints(func)
-
-    # Get the types for header, cookie, path, query, form, and body parameters
-    header: Optional[Type[BaseModel]] = annotations.get("header")
-    cookie: Optional[Type[BaseModel]] = annotations.get("cookie")
-    path: Optional[Type[BaseModel]] = annotations.get("path")
-    query: Optional[Type[BaseModel]] = annotations.get("query")
-    form: Optional[Type[BaseModel]] = annotations.get("form")
-    body: Optional[Type[BaseModel]] = annotations.get("body")
-    raw: Optional[Type[RawModel]] = annotations.get("raw")
-
-    # If doc_ui is False, return the types without further processing
-    if doc_ui is False:
-        return header, cookie, path, query, form, body, raw
-
-    parameters = []
-
-    # If components_schemas is None, initialize it as an empty dictionary
-    if components_schemas is None:
-        components_schemas = dict()
-
-    # If operation is None, initialize it as an Operation object
-    if operation is None:
-        operation = Operation()
-
-    if header:
-        _parameters, _components_schemas = parse_header(header)
-        parameters.extend(_parameters)
-        components_schemas.update(**_components_schemas)
-
-    if cookie:
-        _parameters, _components_schemas = parse_cookie(cookie)
-        parameters.extend(_parameters)
-        components_schemas.update(**_components_schemas)
-
-    if path:
-        _parameters, _components_schemas = parse_path(path)
-        parameters.extend(_parameters)
-        components_schemas.update(**_components_schemas)
-
-    if query:
-        _parameters, _components_schemas = parse_query(query)
-        parameters.extend(_parameters)
-        components_schemas.update(**_components_schemas)
-
-    if form:
-        _content, _components_schemas = parse_form(form)
-        components_schemas.update(**_components_schemas)
-        request_body = RequestBody(content=_content)
-        model_config: DefaultDict[str, Any] = form.model_config  # type: ignore
-        openapi_extra = model_config.get("openapi_extra")
-        if openapi_extra:
-            request_body.description = openapi_extra.get("description")
-            request_body.content["multipart/form-data"].example = openapi_extra.get("example")
-            request_body.content["multipart/form-data"].examples = openapi_extra.get("examples")
-            if openapi_extra.get("encoding"):
-                request_body.content["multipart/form-data"].encoding = openapi_extra.get("encoding")
-        operation.requestBody = request_body
-
-    if body:
-        _content, _components_schemas = parse_body(body)
-        components_schemas.update(**_components_schemas)
-        request_body = RequestBody(content=_content)
-        model_config: DefaultDict[str, Any] = body.model_config  # type: ignore
-        openapi_extra = model_config.get("openapi_extra")
-        if openapi_extra:
-            request_body.description = openapi_extra.get("description")
-            request_body.required = openapi_extra.get("required", True)
-            request_body.content["application/json"].example = openapi_extra.get("example")
-            request_body.content["application/json"].examples = openapi_extra.get("examples")
-            request_body.content["application/json"].encoding = openapi_extra.get("encoding")
-        operation.requestBody = request_body
-
-    if raw:
-        _content = {}
-        for mimetype in raw.mimetypes:
-            if mimetype.startswith("application/json"):
-                _content[mimetype] = MediaType(
-                    schema=Schema(type=DataType.OBJECT)
-                )
-            else:
-                _content[mimetype] = MediaType(
-                    schema=Schema(type=DataType.STRING)
-                )
-        request_body = RequestBody(content=_content)
-        operation.requestBody = request_body
-
-    # Set the parsed parameters in the operation object
-    operation.parameters = parameters if parameters else None
-
-    return header, cookie, path, query, form, body, raw
-
-
-def parse_method(uri: str, method: str, paths: dict, operation: Operation) -> None:
-    """
-    Parses the HTTP method and updates the corresponding PathItem object in the paths' dictionary.
-
-    Args:
-        uri: The URI of the API endpoint.
-        method: The HTTP method for the API endpoint.
-        paths: A dictionary containing the API paths and their corresponding PathItem objects.
-        operation: The Operation object to assign to the PathItem.
-
-    Returns:
-        None
-    """
-    # Check the HTTP method and update the PathItem object in the path dictionary
-    if method == HTTPMethod.GET:
-        if not paths.get(uri):
-            paths[uri] = PathItem(get=operation)
-        else:
-            paths[uri].get = operation
-    elif method == HTTPMethod.POST:
-        if not paths.get(uri):
-            paths[uri] = PathItem(post=operation)
-        else:
-            paths[uri].post = operation
-    elif method == HTTPMethod.PUT:
-        if not paths.get(uri):
-            paths[uri] = PathItem(put=operation)
-        else:
-            paths[uri].put = operation
-    elif method == HTTPMethod.PATCH:
-        if not paths.get(uri):
-            paths[uri] = PathItem(patch=operation)
-        else:
-            paths[uri].patch = operation
-    elif method == HTTPMethod.DELETE:
-        if not paths.get(uri):
-            paths[uri] = PathItem(delete=operation)
-        else:
-            paths[uri].delete = operation
-
-
-def make_validation_error_response(e: ValidationError) -> FlaskResponse:
-    """
-    Create a Flask response for a validation error.
-
-    Args:
-        e: The ValidationError object containing the details of the error.
-
-    Returns:
-        FlaskResponse: A Flask Response object with the JSON representation of the error.
-    """
-    response = make_response(e.json())
-    response.headers["Content-Type"] = "application/json"
-    response.status_code = getattr(current_app, "validation_error_status", 422)
-    return response
-
-
-def parse_rule(rule: str, url_prefix=None) -> str:
-    trail_slash = rule.endswith("/")
-
-    # Merge url_prefix and uri
-    uri = url_prefix.rstrip("/") + "/" + rule.lstrip("/") if url_prefix else rule
-
-    if not trail_slash:
-        uri = uri.rstrip("/")
-
-    # Convert a route parameter format from /pet/<petId> to /pet/{petId}
-    uri = re.sub(r"<([^<:]+:)?", "{", uri).replace(">", "}")
-
-    return uri
-
-
-def convert_responses_key_to_string(responses: ResponseDict) -> ResponseStrKeyDict:
-    """Convert key to string"""
-    _responses = {}
-    for key, value in responses.items():
-        if isinstance(key, HTTPStatus):
-            key = str(key.value)
-        elif isinstance(key, int):
-            key = str(key)
-        _responses[key] = value
-
-    return _responses
-
-
-def normalize_name(name: str) -> str:
-    return re.sub(r"[^\w.\-]", "_", name)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/5/1 21:34
+
+import inspect
+import re
+import sys
+from enum import Enum
+from http import HTTPStatus
+from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional, Any, DefaultDict
+
+from flask import make_response, current_app
+from flask.wrappers import Response as FlaskResponse
+from pydantic import BaseModel, ValidationError
+from pydantic.json_schema import JsonSchemaMode
+
+from .models import Encoding
+from .models import MediaType
+from .models import OPENAPI3_REF_PREFIX
+from .models import OPENAPI3_REF_TEMPLATE
+from .models import Operation
+from .models import Parameter
+from .models import ParameterInType
+from .models import PathItem
+from .models import RawModel
+from .models import RequestBody
+from .models import Response
+from .models import Schema
+from .models import Tag
+from .models.data_type import DataType
+from .types import ParametersTuple
+from .types import ResponseDict
+from .types import ResponseStrKeyDict
+
+HTTP_STATUS = {str(status.value): status.phrase for status in HTTPStatus}
+
+if sys.version_info < (3, 11):
+
+    class HTTPMethod(str, Enum):
+        GET = "GET"
+        POST = "POST"
+        PUT = "PUT"
+        DELETE = "DELETE"
+        PATCH = "PATCH"
+        HEAD = "HEAD"
+        OPTIONS = "OPTIONS"
+        TRACE = "TRACE"
+        CONNECT = "CONNECT"
+else:
+    from http import HTTPMethod
+
+
+def get_operation(
+        func: Callable, *,
+        summary: Optional[str] = None,
+        description: Optional[str] = None,
+        openapi_extensions: Optional[Dict[str, Any]] = None,
+) -> Operation:
+    """
+    Return an Operation object with the specified summary and description.
+
+    Args:
+        func: The function or method for which the operation is being defined.
+        summary: A short summary of what the operation does.
+        description: A verbose explanation of the operation behavior.
+        openapi_extensions: Additional extensions to the OpenAPI Schema.
+
+    Returns:
+        An Operation object representing the operation.
+
+    """
+    # Get the docstring of the function
+    doc = inspect.getdoc(func) or ""
+    doc = doc.strip()
+    lines = doc.split("\n")
+    doc_summary = lines[0] or None
+
+    # Determine the summary and description based on provided arguments or docstring
+    if summary is None:
+        doc_description = lines[0] if len(lines) == 0 else "</br>".join(lines[1:]) or None
+    else:
+        doc_description = "</br>".join(lines) or None
+
+    # Create the operation dictionary with summary and description
+    operation_dict = dict(
+        summary=summary or doc_summary,
+        description=description or doc_description
+    )
+
+    # Add any additional openapi_extensions to the operation dictionary
+    openapi_extensions = openapi_extensions or {}
+    operation_dict.update(**openapi_extensions)
+
+    # Create and return the Operation object
+    operation = Operation(**operation_dict)
+
+    return operation
+
+
+def get_operation_id_for_path(*, name: str, path: str, method: str) -> str:
+    """
+    Generate a unique operation ID based on the name, path, and method.
+
+    Args:
+        name: The name or identifier for the operation.
+        path: The URL path for the operation.
+        method: The HTTP method for the operation.
+
+    Returns:
+        A unique operation ID generated based on the provided name, path, and method.
+
+    """
+    operation_id = name + path
+    # Replace non-word characters with underscores
+    operation_id = re.sub(r"\W", "_", operation_id)
+    operation_id = operation_id + "_" + method.lower()
+    return operation_id
+
+
+def get_model_schema(model: Type[BaseModel], mode: JsonSchemaMode = "validation") -> dict:
+    """Converts a Pydantic model to an OpenAPI schema."""
+
+    assert inspect.isclass(model) and issubclass(model, BaseModel), \
+        f"{model} is invalid `pydantic.BaseModel`"
+
+    model_config = model.model_config
+    by_alias = bool(model_config.get("by_alias", True))
+
+    return model.model_json_schema(by_alias=by_alias, ref_template=OPENAPI3_REF_TEMPLATE, mode=mode)
+
+
+def parse_header(header: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
+    """Parses a header model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(header)
+    parameters = []
+    components_schemas: Dict = dict()
+    properties = schema.get("properties", {})
+
+    for name, value in properties.items():
+        data = {
+            "name": name,
+            "in": ParameterInType.HEADER,
+            "description": value.get("description"),
+            "required": name in schema.get("required", []),
+            "schema": Schema(**value)
+        }
+        # Parse extra values
+        data.update({
+            "deprecated": value.get("deprecated"),
+            "example": value.get("example"),
+            "examples": value.get("examples"),
+        })
+        parameters.append(Parameter(**data))
+
+    # Parse definitions
+    definitions = schema.get("$defs", {})
+    for name, value in definitions.items():
+        components_schemas[name] = Schema(**value)
+
+    return parameters, components_schemas
+
+
+def parse_cookie(cookie: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
+    """Parses a cookie model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(cookie)
+    parameters = []
+    components_schemas: Dict = dict()
+    properties = schema.get("properties", {})
+
+    for name, value in properties.items():
+        data = {
+            "name": name,
+            "in": ParameterInType.COOKIE,
+            "description": value.get("description"),
+            "required": name in schema.get("required", []),
+            "schema": Schema(**value)
+        }
+        # Parse extra values
+        data.update({
+            "deprecated": value.get("deprecated"),
+            "example": value.get("example"),
+            "examples": value.get("examples"),
+        })
+        parameters.append(Parameter(**data))
+
+    # Parse definitions
+    definitions = schema.get("$defs", {})
+    for name, value in definitions.items():
+        components_schemas[name] = Schema(**value)
+
+    return parameters, components_schemas
+
+
+def parse_path(path: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
+    """Parses a path model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(path)
+    parameters = []
+    components_schemas: Dict = dict()
+    properties = schema.get("properties", {})
+
+    for name, value in properties.items():
+        data = {
+            "name": name,
+            "in": ParameterInType.PATH,
+            "description": value.get("description"),
+            "required": True,
+            "schema": Schema(**value)
+        }
+        # Parse extra values
+        data.update({
+            "deprecated": value.get("deprecated"),
+            "example": value.get("example"),
+            "examples": value.get("examples"),
+        })
+        parameters.append(Parameter(**data))
+
+    # Parse definitions
+    definitions = schema.get("$defs", {})
+    for name, value in definitions.items():
+        components_schemas[name] = Schema(**value)
+
+    return parameters, components_schemas
+
+
+def parse_query(query: Type[BaseModel]) -> Tuple[List[Parameter], dict]:
+    """Parses a query model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(query)
+    parameters = []
+    components_schemas: Dict = dict()
+    properties = schema.get("properties", {})
+
+    for name, value in properties.items():
+        data = {
+            "name": name,
+            "in": ParameterInType.QUERY,
+            "description": value.get("description"),
+            "required": name in schema.get("required", []),
+            "schema": Schema(**value)
+        }
+        # Parse extra values
+        data.update({
+            "deprecated": value.get("deprecated"),
+            "example": value.get("example"),
+            "examples": value.get("examples"),
+        })
+        parameters.append(Parameter(**data))
+
+    # Parse definitions
+    definitions = schema.get("$defs", {})
+    for name, value in definitions.items():
+        components_schemas[name] = Schema(**value)
+
+    return parameters, components_schemas
+
+
+def parse_form(
+        form: Type[BaseModel],
+) -> Tuple[Dict[str, MediaType], dict]:
+    """Parses a form model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(form)
+    components_schemas = dict()
+    properties = schema.get("properties", {})
+
+    assert properties, f"{form.__name__}'s properties cannot be empty."
+
+    original_title = schema.get("title") or form.__name__
+    title = normalize_name(original_title)
+    components_schemas[title] = Schema(**schema)
+    encoding = {}
+    for k, v in properties.items():
+        if v.get("type") == "array":
+            encoding[k] = Encoding(style="form", explode=True)
+    content = {
+        "multipart/form-data": MediaType(
+            schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"}),
+            encoding=encoding or None
+        )
+    }
+
+    # Parse definitions
+    definitions = schema.get("$defs", {})
+    for name, value in definitions.items():
+        components_schemas[name] = Schema(**value)
+
+    return content, components_schemas
+
+
+def parse_body(
+        body: Type[BaseModel],
+) -> Tuple[Dict[str, MediaType], dict]:
+    """Parses a body model and returns a list of parameters and component schemas."""
+    schema = get_model_schema(body)
+    components_schemas = dict()
+
+    original_title = schema.get("title") or body.__name__
+    title = normalize_name(original_title)
+    components_schemas[title] = Schema(**schema)
+    content = {
+        "application/json": MediaType(
+            schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{title}"})
+        )
+    }
+
+    # Parse definitions
+    definitions = schema.get("$defs", {})
+    for name, value in definitions.items():
+        components_schemas[name] = Schema(**value)
+
+    return content, components_schemas
+
+
+def get_responses(
+        responses: ResponseStrKeyDict,
+        components_schemas: dict,
+        operation: Operation
+) -> None:
+    _responses = {}
+    _schemas = {}
+
+    for key, response in responses.items():
+        if response is None:
+            # If the response is None, it means HTTP status code "204" (No Content)
+            _responses[key] = Response(description=HTTP_STATUS.get(key, ""))
+        elif isinstance(response, dict):
+            if not response.get("description"):
+                response["description"] = HTTP_STATUS.get(key, "")
+            _responses[key] = Response(**response)
+        else:
+            # OpenAPI 3 support ^[a-zA-Z0-9\.\-_]+$ so we should normalize __name__
+            name = normalize_name(response.__name__)
+            schema = get_model_schema(response, mode="serialization")
+            _responses[key] = Response(
+                description=HTTP_STATUS.get(key, ""),
+                content={
+                    "application/json": MediaType(
+                        schema=Schema(**{"$ref": f"{OPENAPI3_REF_PREFIX}/{name}"})
+                    )})
+
+            model_config: DefaultDict[str, Any] = response.model_config  # type: ignore
+            openapi_extra = model_config.get("openapi_extra")
+            if openapi_extra:
+                # Add additional information from model_config to the response
+                _responses[key].description = openapi_extra.get("description")
+                _responses[key].headers = openapi_extra.get("headers")
+                _responses[key].links = openapi_extra.get("links")
+                _content = _responses[key].content
+                if _content is not None:
+                    _content["application/json"].example = openapi_extra.get("example")
+                    _content["application/json"].examples = openapi_extra.get("examples")
+                    _content["application/json"].encoding = openapi_extra.get("encoding")
+                    _content.update(openapi_extra.get("content", {}))
+
+            _schemas[name] = Schema(**schema)
+            definitions = schema.get("$defs")
+            if definitions:
+                # Add schema definitions to _schemas
+                for name, value in definitions.items():
+                    _schemas[normalize_name(name)] = Schema(**value)
+
+    components_schemas.update(**_schemas)
+    operation.responses = _responses
+
+
+def parse_and_store_tags(
+        new_tags: List[Tag],
+        old_tags: List[Tag],
+        old_tag_names: List[str],
+        operation: Operation
+) -> None:
+    """
+    Parses new tags, stores them in an old_tags list if they are not already present,
+    and updates the tags attribute of the operation object.
+
+    Args:
+        new_tags: A list of new Tag objects to be parsed and stored.
+        old_tags: The list of existing Tag objects.
+        old_tag_names: The list that names of existing tags.
+        operation: The operation object whose tag attribute needs to be updated.
+
+    Returns:
+        None
+    """
+    # Iterate over each tag in new_tags
+    for tag in new_tags:
+        if tag.name not in old_tag_names:
+            old_tag_names.append(tag.name)
+            old_tags.append(tag)
+
+    # Set the tags attribute of the operation object to a list of unique tag names from new_tags
+    # If the resulting list is empty, set it to None
+    operation.tags = list(set([tag.name for tag in new_tags])) or None
+
+
+def parse_parameters(
+        func: Callable,
+        *,
+        components_schemas: Optional[Dict] = None,
+        operation: Optional[Operation] = None,
+        doc_ui: bool = True,
+) -> ParametersTuple:
+    """
+    Parses the parameters of a given function and returns the types for header, cookie, path,
+    query, form, and body parameters. Also populates the Operation object with the parsed parameters.
+
+    Args:
+        func: The function to parse the parameters from.
+        components_schemas: Dictionary to store the parsed components schemas (default: None).
+        operation: Operation object to populate with parsed parameters (default: None).
+        doc_ui: Flag indicating whether to return types for documentation UI (default: True).
+
+    Returns:
+        Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
+        The types for header, cookie, path, query, form, and body parameters respectively.
+
+    """
+    # Get the type hints from the function
+    annotations = get_type_hints(func)
+
+    # Get the types for header, cookie, path, query, form, and body parameters
+    header: Optional[Type[BaseModel]] = annotations.get("header")
+    cookie: Optional[Type[BaseModel]] = annotations.get("cookie")
+    path: Optional[Type[BaseModel]] = annotations.get("path")
+    query: Optional[Type[BaseModel]] = annotations.get("query")
+    form: Optional[Type[BaseModel]] = annotations.get("form")
+    body: Optional[Type[BaseModel]] = annotations.get("body")
+    raw: Optional[Type[RawModel]] = annotations.get("raw")
+
+    # If doc_ui is False, return the types without further processing
+    if doc_ui is False:
+        return header, cookie, path, query, form, body, raw
+
+    parameters = []
+
+    # If components_schemas is None, initialize it as an empty dictionary
+    if components_schemas is None:
+        components_schemas = dict()
+
+    # If operation is None, initialize it as an Operation object
+    if operation is None:
+        operation = Operation()
+
+    if header:
+        _parameters, _components_schemas = parse_header(header)
+        parameters.extend(_parameters)
+        components_schemas.update(**_components_schemas)
+
+    if cookie:
+        _parameters, _components_schemas = parse_cookie(cookie)
+        parameters.extend(_parameters)
+        components_schemas.update(**_components_schemas)
+
+    if path:
+        _parameters, _components_schemas = parse_path(path)
+        parameters.extend(_parameters)
+        components_schemas.update(**_components_schemas)
+
+    if query:
+        _parameters, _components_schemas = parse_query(query)
+        parameters.extend(_parameters)
+        components_schemas.update(**_components_schemas)
+
+    if form:
+        _content, _components_schemas = parse_form(form)
+        components_schemas.update(**_components_schemas)
+        request_body = RequestBody(content=_content)
+        model_config: DefaultDict[str, Any] = form.model_config  # type: ignore
+        openapi_extra = model_config.get("openapi_extra")
+        if openapi_extra:
+            request_body.description = openapi_extra.get("description")
+            request_body.content["multipart/form-data"].example = openapi_extra.get("example")
+            request_body.content["multipart/form-data"].examples = openapi_extra.get("examples")
+            if openapi_extra.get("encoding"):
+                request_body.content["multipart/form-data"].encoding = openapi_extra.get("encoding")
+        operation.requestBody = request_body
+
+    if body:
+        _content, _components_schemas = parse_body(body)
+        components_schemas.update(**_components_schemas)
+        request_body = RequestBody(content=_content)
+        model_config: DefaultDict[str, Any] = body.model_config  # type: ignore
+        openapi_extra = model_config.get("openapi_extra")
+        if openapi_extra:
+            request_body.description = openapi_extra.get("description")
+            request_body.required = openapi_extra.get("required", True)
+            request_body.content["application/json"].example = openapi_extra.get("example")
+            request_body.content["application/json"].examples = openapi_extra.get("examples")
+            request_body.content["application/json"].encoding = openapi_extra.get("encoding")
+        operation.requestBody = request_body
+
+    if raw:
+        _content = {}
+        for mimetype in raw.mimetypes:
+            if mimetype.startswith("application/json"):
+                _content[mimetype] = MediaType(
+                    schema=Schema(type=DataType.OBJECT)
+                )
+            else:
+                _content[mimetype] = MediaType(
+                    schema=Schema(type=DataType.STRING)
+                )
+        request_body = RequestBody(content=_content)
+        operation.requestBody = request_body
+
+    # Set the parsed parameters in the operation object
+    operation.parameters = parameters if parameters else None
+
+    return header, cookie, path, query, form, body, raw
+
+
+def parse_method(uri: str, method: str, paths: dict, operation: Operation) -> None:
+    """
+    Parses the HTTP method and updates the corresponding PathItem object in the paths' dictionary.
+
+    Args:
+        uri: The URI of the API endpoint.
+        method: The HTTP method for the API endpoint.
+        paths: A dictionary containing the API paths and their corresponding PathItem objects.
+        operation: The Operation object to assign to the PathItem.
+
+    Returns:
+        None
+    """
+    # Check the HTTP method and update the PathItem object in the path dictionary
+    if method == HTTPMethod.GET:
+        if not paths.get(uri):
+            paths[uri] = PathItem(get=operation)
+        else:
+            paths[uri].get = operation
+    elif method == HTTPMethod.POST:
+        if not paths.get(uri):
+            paths[uri] = PathItem(post=operation)
+        else:
+            paths[uri].post = operation
+    elif method == HTTPMethod.PUT:
+        if not paths.get(uri):
+            paths[uri] = PathItem(put=operation)
+        else:
+            paths[uri].put = operation
+    elif method == HTTPMethod.PATCH:
+        if not paths.get(uri):
+            paths[uri] = PathItem(patch=operation)
+        else:
+            paths[uri].patch = operation
+    elif method == HTTPMethod.DELETE:
+        if not paths.get(uri):
+            paths[uri] = PathItem(delete=operation)
+        else:
+            paths[uri].delete = operation
+
+
+def make_validation_error_response(e: ValidationError) -> FlaskResponse:
+    """
+    Create a Flask response for a validation error.
+
+    Args:
+        e: The ValidationError object containing the details of the error.
+
+    Returns:
+        FlaskResponse: A Flask Response object with the JSON representation of the error.
+    """
+    response = make_response(e.json())
+    response.headers["Content-Type"] = "application/json"
+    response.status_code = getattr(current_app, "validation_error_status", 422)
+    return response
+
+
+def parse_rule(rule: str, url_prefix=None) -> str:
+    trail_slash = rule.endswith("/")
+
+    # Merge url_prefix and uri
+    uri = url_prefix.rstrip("/") + "/" + rule.lstrip("/") if url_prefix else rule
+
+    if not trail_slash:
+        uri = uri.rstrip("/")
+
+    # Convert a route parameter format from /pet/<petId> to /pet/{petId}
+    uri = re.sub(r"<([^<:]+:)?", "{", uri).replace(">", "}")
+
+    return uri
+
+
+def convert_responses_key_to_string(responses: ResponseDict) -> ResponseStrKeyDict:
+    """Convert key to string"""
+    _responses = {}
+    for key, value in responses.items():
+        if isinstance(key, HTTPStatus):
+            key = str(key.value)
+        elif isinstance(key, int):
+            key = str(key)
+        _responses[key] = value
+
+    return _responses
+
+
+def normalize_name(name: str) -> str:
+    return re.sub(r"[^\w.\-]", "_", name)
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/view.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/blueprint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,215 +1,198 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/10/14 16:09
-import typing
-from copy import deepcopy
-from typing import Optional, List, Dict, Any, Callable
-
-from .models import ExternalDocumentation
-from .models import Server
-from .models import Tag
-from .types import ResponseDict
-from .utils import HTTPMethod
-from .utils import convert_responses_key_to_string
-from .utils import get_operation
-from .utils import get_operation_id_for_path
-from .utils import get_responses
-from .utils import parse_and_store_tags
-from .utils import parse_method
-from .utils import parse_parameters
-from .utils import parse_rule
-
-if typing.TYPE_CHECKING:
-    from .openapi import OpenAPI
-
-
-class APIView:
-    def __init__(
-            self,
-            url_prefix: Optional[str] = None,
-            view_tags: Optional[List[Tag]] = None,
-            view_security: Optional[List[Dict[str, List[str]]]] = None,
-            view_responses: Optional[ResponseDict] = None,
-            doc_ui: bool = True,
-            operation_id_callback: Callable = get_operation_id_for_path,
-    ):
-        """
-        Create a class-based view
-
-        Args:
-            url_prefix: A path to prepend to all the APIView's urls
-            view_tags: APIView tags for every API.
-            view_security: APIView security for every API.
-            view_responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            doc_ui: Enable OpenAPI document UI (Swagger UI and Redoc). Defaults to True.
-            operation_id_callback: Callback function for custom operation_id generation.
-                                   Receives name (str), path (str) and method (str) parameters.
-                                   Defaults to `get_operation_id_for_path` from utils
-        """
-        self.url_prefix = url_prefix
-        self.view_tags = view_tags or []
-        self.view_security = view_security or []
-
-        view_responses = view_responses or {}
-        # Convert key to string
-        self.view_responses = convert_responses_key_to_string(view_responses)
-
-        self.doc_ui = doc_ui
-        self.operation_id_callback: Callable = operation_id_callback
-
-        self.views: Dict = dict()
-        self.paths: Dict = dict()
-        self.components_schemas: Dict = dict()
-        self.tags: List[Tag] = []
-        self.tag_names: List[str] = []
-
-    def route(self, rule: str):
-        """Decorator for view class"""
-
-        def wrapper(cls):
-            if self.views.get(rule):
-                raise ValueError(f"malformed url rule: {rule!r}")
-            methods = []
-
-            # Parse rule: merge url_prefix and format rule from /pet/<petId> to /pet/{petId}
-            uri = parse_rule(rule, url_prefix=self.url_prefix)
-
-            for method in HTTPMethod:
-                cls_method = getattr(cls, method.lower(), None)
-                if not cls_method:
-                    continue
-                methods.append(method)
-                if self.doc_ui is False:
-                    continue
-                if not getattr(cls_method, "operation", None):
-                    continue
-                # Parse method
-                parse_method(uri, method, self.paths, cls_method.operation)
-                # Update operation_id
-                if not cls_method.operation.operationId:
-                    cls_method.operation.operationId = self.operation_id_callback(
-                        name=cls_method.__qualname__,
-                        path=rule,
-                        method=method
-                    )
-
-            # Convert route parameters from {param} to <param>
-            _rule = uri.replace("{", "<").replace("}", ">")
-            self.views[_rule] = (cls, methods)
-
-            return cls
-
-        return wrapper
-
-    def doc(
-            self,
-            *,
-            tags: Optional[List[Tag]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            external_docs: Optional[ExternalDocumentation] = None,
-            operation_id: Optional[str] = None,
-            responses: Optional[ResponseDict] = None,
-            deprecated: Optional[bool] = None,
-            security: Optional[List[Dict[str, List[Any]]]] = None,
-            servers: Optional[List[Server]] = None,
-            openapi_extensions: Optional[Dict[str, Any]] = None,
-            doc_ui: bool = True
-    ) -> Callable:
-        """
-        Decorator for view method.
-        More information goto https://spec.openapis.org/oas/v3.1.0#operation-object
-
-        Args:
-            tags: Adds metadata to a single tag.
-            summary: A short summary of what the operation does.
-            description: A verbose explanation of the operation behavior.
-            external_docs: Additional external documentation for this operation.
-            operation_id: Unique string used to identify the operation.
-            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
-            deprecated: Declares this operation to be deprecated.
-            security: A declaration of which security mechanisms can be used for this operation.
-            servers: An alternative server array to service this operation.
-            openapi_extensions: Allows extensions to the OpenAPI Schema.
-            doc_ui: Declares this operation to be shown. Default to True.
-        """
-
-        if responses is None:
-            new_responses = {}
-        else:
-            # Convert key to string
-            new_responses = convert_responses_key_to_string(responses)
-        if security is None:
-            security = []
-        tags = tags + self.view_tags if tags else self.view_tags
-
-        def decorator(func):
-            if self.doc_ui is False or doc_ui is False:
-                return
-            # Global response combines API responses
-            combine_responses = deepcopy(self.view_responses)
-            combine_responses.update(**new_responses)
-            # Create operation
-            operation = get_operation(
-                func,
-                summary=summary,
-                description=description,
-                openapi_extensions=openapi_extensions
-            )
-            # Set external docs
-            operation.externalDocs = external_docs
-            # Unique string used to identify the operation.
-            operation.operationId = operation_id
-            # Only set `deprecated` if True, otherwise leave it as None
-            operation.deprecated = deprecated
-            # Add security
-            operation.security = security + self.view_security or None
-            # Add servers
-            operation.servers = servers
-            # Store tags
-            parse_and_store_tags(tags, self.tags, self.tag_names, operation)
-            # Parse parameters
-            parse_parameters(
-                func,
-                components_schemas=self.components_schemas,
-                operation=operation
-            )
-            # Parse response
-            get_responses(combine_responses, self.components_schemas, operation)
-            func.operation = operation
-
-            return func
-
-        return decorator
-
-    def register(self, app: "OpenAPI", view_kwargs: Optional[Dict[Any, Any]] = None) -> None:
-        """
-        Register the API views with the given OpenAPI app.
-
-        Args:
-            app: An instance of the OpenAPI app.
-            view_kwargs: Additional keyword arguments to pass to the API views.
-        """
-        if view_kwargs is None:
-            view_kwargs = {}
-        for rule, (cls, methods) in self.views.items():
-            for method in methods:
-                func = getattr(cls, method.lower())
-                header, cookie, path, query, form, body, raw = parse_parameters(func, doc_ui=False)
-                view_func = app.create_view_func(
-                    func,
-                    header,
-                    cookie,
-                    path,
-                    query,
-                    form,
-                    body,
-                    raw,
-                    view_class=cls,
-                    view_kwargs=view_kwargs
-                )
-                options = {
-                    "endpoint": cls.__name__ + "." + method.lower(),
-                    "methods": [method.upper()]
-                }
-                app.add_url_rule(rule, view_func=view_func, **options)
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/4/1 16:54
+from copy import deepcopy
+from typing import Optional, List, Dict, Any, Callable
+
+from flask import Blueprint
+
+from .models import ExternalDocumentation
+from .models import Server
+from .models import Tag
+from .scaffold import APIScaffold
+from .types import ParametersTuple
+from .types import ResponseDict
+from .utils import HTTPMethod
+from .utils import convert_responses_key_to_string
+from .utils import get_operation
+from .utils import get_operation_id_for_path
+from .utils import get_responses
+from .utils import parse_and_store_tags
+from .utils import parse_method
+from .utils import parse_parameters
+from .utils import parse_rule
+
+
+class APIBlueprint(APIScaffold, Blueprint):
+    def __init__(
+            self,
+            name: str,
+            import_name: str,
+            *,
+            abp_tags: Optional[List[Tag]] = None,
+            abp_security: Optional[List[Dict[str, List[str]]]] = None,
+            abp_responses: Optional[ResponseDict] = None,
+            doc_ui: bool = True,
+            operation_id_callback: Callable = get_operation_id_for_path,
+            **kwargs: Any
+    ) -> None:
+        """
+        Based on Flask Blueprint
+
+        Args:
+            name: The name of the blueprint. It Will be prepared to each endpoint name.
+            import_name: The name of the blueprint package, usually ``__name__``.
+                         This helps locate the ``root_path`` for the blueprint.
+            abp_tags: APIBlueprint tags for every API.
+            abp_security: APIBlueprint security for every API.
+            abp_responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            doc_ui: Enable OpenAPI document UI (Swagger UI, Redoc, and Rapidoc). Defaults to True.
+            operation_id_callback: Callback function for custom operation_id generation.
+                                   Receives name (str), path (str) and method (str) parameters.
+                                   Defaults to `get_operation_id_for_path` from utils
+            **kwargs: Flask Blueprint kwargs
+        """
+        super(APIBlueprint, self).__init__(name, import_name, **kwargs)
+
+        # Initialize instance variables
+        self.paths: Dict = dict()
+        self.components_schemas: Dict = dict()
+        self.tags: List[Tag] = []
+        self.tag_names: List[str] = []
+
+        # Set values from arguments or default values
+        self.abp_tags = abp_tags or []
+        self.abp_security = abp_security or []
+
+        abp_responses = abp_responses or {}
+        # Convert key to string
+        self.abp_responses = convert_responses_key_to_string(abp_responses)
+
+        self.doc_ui = doc_ui
+
+        # Set the operation ID callback function
+        self.operation_id_callback: Callable = operation_id_callback
+
+    def register_api(self, api: "APIBlueprint") -> None:
+        """Register a nested APIBlueprint"""
+
+        # Check if the APIBlueprint is being registered on itself
+        if api is self:
+            raise ValueError("Cannot register a api blueprint on itself")
+
+        # Merge tags from the nested APIBlueprint
+        for tag in api.tags:
+            if tag.name not in self.tag_names:
+                self.tags.append(tag)
+
+        # Merge paths from the nested APIBlueprint
+        for path_url, path_item in api.paths.items():
+            # Parse rule: merge url_prefix and format rule from /pet/<petId> to /pet/{petId}
+            uri = parse_rule(path_url, url_prefix=self.url_prefix)
+
+            self.paths[uri] = path_item
+
+        # Merge component schemas from the nested APIBlueprint
+        self.components_schemas.update(**api.components_schemas)
+
+        # Register the nested APIBlueprint as a blueprint
+        self.register_blueprint(api)
+
+    def _add_url_rule(
+            self,
+            rule,
+            endpoint=None,
+            view_func=None,
+            provide_automatic_options=None,
+            **options,
+    ) -> None:
+        self.add_url_rule(rule, endpoint, view_func, provide_automatic_options, **options)
+
+    def _collect_openapi_info(
+            self,
+            rule: str,
+            func: Callable,
+            *,
+            tags: Optional[List[Tag]] = None,
+            summary: Optional[str] = None,
+            description: Optional[str] = None,
+            external_docs: Optional[ExternalDocumentation] = None,
+            operation_id: Optional[str] = None,
+            responses: Optional[ResponseDict] = None,
+            deprecated: Optional[bool] = None,
+            security: Optional[List[Dict[str, List[Any]]]] = None,
+            servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
+            doc_ui: bool = True,
+            method: str = HTTPMethod.GET
+    ) -> ParametersTuple:
+        """
+        Collects OpenAPI specification information for Flask routes and view functions.
+
+        Args:
+            rule: Flask route
+            func: Flask view_func
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            responses: API responses should be either a subclass of BaseModel, a dictionary, or None.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Declares this operation to be shown. Default to True.
+        """
+        if self.doc_ui is True and doc_ui is True:
+            if responses is None:
+                new_responses = {}
+            else:
+                # Convert key to string
+                new_responses = convert_responses_key_to_string(responses)
+            # Global response: combine API responses
+            combine_responses = deepcopy(self.abp_responses)
+            combine_responses.update(**new_responses)
+            # Create operation
+            operation = get_operation(
+                func,
+                summary=summary,
+                description=description,
+                openapi_extensions=openapi_extensions
+            )
+            # Set external docs
+            operation.externalDocs = external_docs
+            # Unique string used to identify the operation.
+            operation.operationId = operation_id or self.operation_id_callback(
+                name=self.name, path=rule, method=method
+            )
+            # Only set `deprecated` if True, otherwise leave it as None
+            operation.deprecated = deprecated
+            # Add security
+            if security is None:
+                security = []
+            operation.security = security + self.abp_security or None
+            # Add servers
+            operation.servers = servers
+            # Store tags
+            tags = tags + self.abp_tags if tags else self.abp_tags
+            parse_and_store_tags(tags, self.tags, self.tag_names, operation)
+            # Parse parameters
+            header, cookie, path, query, form, body, raw = parse_parameters(
+                func,
+                components_schemas=self.components_schemas,
+                operation=operation
+            )
+            # Parse response
+            get_responses(combine_responses, self.components_schemas, operation)
+
+            # Parse rule: merge url_prefix and format rule from /pet/<petId> to /pet/{petId}
+            uri = parse_rule(rule, url_prefix=self.url_prefix)
+
+            # Parse method
+            parse_method(uri, method, self.paths, operation)
+            return header, cookie, path, query, form, body, raw
+        else:
+            # Parse parameters
+            header, cookie, path, query, form, body, raw = parse_parameters(func, doc_ui=False)
+            return header, cookie, path, query, form, body, raw
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/__init__.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/4/28 10:58
-"""
-OpenAPI v3.1.0 schema types, created according to the specification:
-https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md
-
-The type orders are according to the contents of the specification:
-https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md#table-of-contents
-"""
-
-from typing import Optional, List, Dict
-
-from flask import Request
-from pydantic import BaseModel
-
-from .callback import Callback
-from .components import Components
-from .contact import Contact
-from .discriminator import Discriminator
-from .encoding import Encoding
-from .example import Example
-from .external_documentation import ExternalDocumentation
-from .file import FileStorage
-from .header import Header
-from .info import Info
-from .license import License
-from .link import Link
-from .media_type import MediaType
-from .oauth_flow import OAuthFlow
-from .oauth_flows import OAuthFlows
-from .operation import Operation
-from .parameter import Parameter
-from .parameter_in_type import ParameterInType
-from .path_item import PathItem
-from .paths import Paths
-from .reference import Reference
-from .request_body import RequestBody
-from .response import Response
-from .responses import Responses
-from .schema import Schema
-from .security_requirement import SecurityRequirement
-from .security_scheme import SecurityScheme
-from .server import Server
-from .server_variable import ServerVariable
-from .style_values import StyleValues
-from .tag import Tag
-from .validation_error import UnprocessableEntity
-from .validation_error import ValidationErrorModel
-from .xml import XML
-
-OPENAPI3_REF_PREFIX = "#/components/schemas"
-OPENAPI3_REF_TEMPLATE = OPENAPI3_REF_PREFIX + "/{model}"
-
-
-class APISpec(BaseModel):
-    """https://spec.openapis.org/oas/v3.1.0#openapi-object"""
-    openapi: str
-    info: Info
-    servers: Optional[List[Server]] = None
-    paths: Paths
-    components: Optional[Components] = None
-    security: Optional[List[SecurityRequirement]] = None
-    tags: Optional[List[Tag]] = None
-    externalDocs: Optional[ExternalDocumentation] = None
-
-    model_config = {
-        "extra": "allow"
-    }
-
-
-class OAuthConfig(BaseModel):
-    """
-    https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/oauth2.md#oauth-20-configuration
-    """
-    clientId: Optional[str] = None
-    clientSecret: Optional[str] = None
-    realm: Optional[str] = None
-    appName: Optional[str] = None
-    scopeSeparator: Optional[str] = None
-    scopes: Optional[str] = None
-    additionalQueryStringParams: Optional[Dict[str, str]] = None
-    useBasicAuthenticationWithAccessCodeGrant: Optional[bool] = False
-    usePkceWithAuthorizationCodeGrant: Optional[bool] = False
-
-
-class RawModel(Request):
-    mimetypes: List[str] = ["application/json"]
-
-
-Encoding.model_rebuild()
-Operation.model_rebuild()
-PathItem.model_rebuild()
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/4/28 10:58
+"""
+OpenAPI v3.1.0 schema types, created according to the specification:
+https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md
+
+The type orders are according to the contents of the specification:
+https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md#table-of-contents
+"""
+
+from typing import Optional, List, Dict
+
+from flask import Request
+from pydantic import BaseModel
+
+from .callback import Callback
+from .components import Components
+from .contact import Contact
+from .discriminator import Discriminator
+from .encoding import Encoding
+from .example import Example
+from .external_documentation import ExternalDocumentation
+from .file import FileStorage
+from .header import Header
+from .info import Info
+from .license import License
+from .link import Link
+from .media_type import MediaType
+from .oauth_flow import OAuthFlow
+from .oauth_flows import OAuthFlows
+from .operation import Operation
+from .parameter import Parameter
+from .parameter_in_type import ParameterInType
+from .path_item import PathItem
+from .paths import Paths
+from .reference import Reference
+from .request_body import RequestBody
+from .response import Response
+from .responses import Responses
+from .schema import Schema
+from .security_requirement import SecurityRequirement
+from .security_scheme import SecurityScheme
+from .server import Server
+from .server_variable import ServerVariable
+from .style_values import StyleValues
+from .tag import Tag
+from .validation_error import UnprocessableEntity
+from .validation_error import ValidationErrorModel
+from .xml import XML
+
+OPENAPI3_REF_PREFIX = "#/components/schemas"
+OPENAPI3_REF_TEMPLATE = OPENAPI3_REF_PREFIX + "/{model}"
+
+
+class APISpec(BaseModel):
+    """https://spec.openapis.org/oas/v3.1.0#openapi-object"""
+    openapi: str
+    info: Info
+    servers: Optional[List[Server]] = None
+    paths: Paths
+    components: Optional[Components] = None
+    security: Optional[List[SecurityRequirement]] = None
+    tags: Optional[List[Tag]] = None
+    externalDocs: Optional[ExternalDocumentation] = None
+
+    model_config = {
+        "extra": "allow"
+    }
+
+
+class OAuthConfig(BaseModel):
+    """
+    https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/oauth2.md#oauth-20-configuration
+    """
+    clientId: Optional[str] = None
+    clientSecret: Optional[str] = None
+    realm: Optional[str] = None
+    appName: Optional[str] = None
+    scopeSeparator: Optional[str] = None
+    scopes: Optional[str] = None
+    additionalQueryStringParams: Optional[Dict[str, str]] = None
+    useBasicAuthenticationWithAccessCodeGrant: Optional[bool] = False
+    usePkceWithAuthorizationCodeGrant: Optional[bool] = False
+
+
+class RawModel(Request):
+    mimetypes: List[str] = ["application/json"]
+
+
+Encoding.model_rebuild()
+Operation.model_rebuild()
+PathItem.model_rebuild()
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/components.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/components.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:36
-from typing import Dict, Optional, Union, Any
-
-from pydantic import BaseModel, Field
-
-from .callback import Callback
-from .example import Example
-from .header import Header
-from .link import Link
-from .parameter import Parameter
-from .path_item import PathItem
-from .reference import Reference
-from .request_body import RequestBody
-from .response import Response
-from .schema import Schema
-from .security_scheme import SecurityScheme
-
-
-class Components(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#components-object
-    """
-
-    schemas: Optional[Dict[str, Union[Reference, Schema]]] = Field(None)
-    responses: Optional[Dict[str, Union[Response, Reference]]] = None
-    parameters: Optional[Dict[str, Union[Parameter, Reference]]] = None
-    examples: Optional[Dict[str, Union[Example, Reference]]] = None
-    requestBodies: Optional[Dict[str, Union[RequestBody, Reference]]] = None
-    headers: Optional[Dict[str, Union[Header, Reference]]] = None
-    securitySchemes: Optional[Dict[str, Union[SecurityScheme, Dict[str, Any]]]] = None
-    links: Optional[Dict[str, Union[Link, Reference]]] = None
-    callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
-    pathItems: Optional[Dict[str, Union[PathItem, Reference]]] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:36
+from typing import Dict, Optional, Union, Any
+
+from pydantic import BaseModel, Field
+
+from .callback import Callback
+from .example import Example
+from .header import Header
+from .link import Link
+from .parameter import Parameter
+from .path_item import PathItem
+from .reference import Reference
+from .request_body import RequestBody
+from .response import Response
+from .schema import Schema
+from .security_scheme import SecurityScheme
+
+
+class Components(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#components-object
+    """
+
+    schemas: Optional[Dict[str, Union[Reference, Schema]]] = Field(None)
+    responses: Optional[Dict[str, Union[Response, Reference]]] = None
+    parameters: Optional[Dict[str, Union[Parameter, Reference]]] = None
+    examples: Optional[Dict[str, Union[Example, Reference]]] = None
+    requestBodies: Optional[Dict[str, Union[RequestBody, Reference]]] = None
+    headers: Optional[Dict[str, Union[Header, Reference]]] = None
+    securitySchemes: Optional[Dict[str, Union[SecurityScheme, Dict[str, Any]]]] = None
+    links: Optional[Dict[str, Union[Link, Reference]]] = None
+    callbacks: Optional[Dict[str, Union[Callback, Reference]]] = None
+    pathItems: Optional[Dict[str, Union[PathItem, Reference]]] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/encoding.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:41
-from typing import TYPE_CHECKING, Dict, Optional, Union
-
-from pydantic import BaseModel
-
-from .reference import Reference
-
-if TYPE_CHECKING:
-    from .header import Header
-else:
-    Header = "Header"
-
-
-class Encoding(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#encoding-object
-    """
-
-    contentType: Optional[str] = None
-    headers: Optional[Dict[str, Union[Header, Reference]]] = None
-    style: Optional[str] = None
-    explode: Optional[bool] = None
-    allowReserved: bool = False
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/4/28 10:58
+from typing import Optional
+
+from pydantic import BaseModel
+
+from .contact import Contact
+from .license import License
+
+
+class Info(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#info-object
+    """
+
+    title: str
+    summary: Optional[str] = None
+    description: Optional[str] = None
+    termsOfService: Optional[str] = None
+    contact: Optional[Contact] = None
+    license: Optional[License] = None
+    version: str
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/file.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/file.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/5/11 16:17
-from typing import Any
-
-from pydantic.json_schema import JsonSchemaValue
-from pydantic_core import core_schema
-from werkzeug.datastructures import FileStorage as _FileStorage
-
-
-class FileStorage(_FileStorage):
-    """
-    An uploaded file included as part of the request data.
-    """
-
-    @classmethod
-    def __get_pydantic_json_schema__(cls, _core_schema, _handler) -> JsonSchemaValue:
-        field_schema = {"format": "binary", "type": "string"}
-        return field_schema
-
-    @classmethod
-    def __get_pydantic_core_schema__(cls, _source: Any) -> core_schema.CoreSchema:
-        return core_schema.with_info_plain_validator_function(cls.validate)
-
-    @classmethod
-    def validate(cls, value: _FileStorage, _info: core_schema.ValidationInfo) -> _FileStorage:
-        return value
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/5/11 16:17
+from typing import Any
+
+from pydantic.json_schema import JsonSchemaValue
+from pydantic_core import core_schema
+from werkzeug.datastructures import FileStorage as _FileStorage
+
+
+class FileStorage(_FileStorage):
+    """
+    An uploaded file included as part of the request data.
+    """
+
+    @classmethod
+    def __get_pydantic_json_schema__(cls, _core_schema, _handler) -> JsonSchemaValue:
+        field_schema = {"format": "binary", "type": "string"}
+        return field_schema
+
+    @classmethod
+    def __get_pydantic_core_schema__(cls, _source: Any) -> core_schema.CoreSchema:
+        return core_schema.with_info_plain_validator_function(cls.validate)
+
+    @classmethod
+    def validate(cls, value: _FileStorage, _info: core_schema.ValidationInfo) -> _FileStorage:
+        return value
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/link.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/link.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:45
-from typing import Any, Dict, Optional
-
-from pydantic import BaseModel
-
-from .server import Server
-
-
-class Link(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#link-object
-    """
-
-    operationRef: Optional[str] = None
-    operationId: Optional[str] = None
-    parameters: Optional[Dict[str, Any]] = None
-    requestBody: Optional[Any] = None
-    description: Optional[str] = None
-    server: Optional[Server] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:45
+from typing import Any, Dict, Optional
+
+from pydantic import BaseModel
+
+from .server import Server
+
+
+class Link(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#link-object
+    """
+
+    operationRef: Optional[str] = None
+    operationId: Optional[str] = None
+    parameters: Optional[Dict[str, Any]] = None
+    requestBody: Optional[Any] = None
+    description: Optional[str] = None
+    server: Optional[Server] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/media_type.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/media_type.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:46
-from typing import Any, Dict, Optional, Union
-
-from pydantic import BaseModel, Field
-
-from .encoding import Encoding
-from .example import Example
-from .reference import Reference
-from .schema import Schema
-
-
-class MediaType(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#media-type-object
-    """
-
-    media_type_schema: Optional[Union[Reference, Schema]] = Field(default=None, alias="schema")
-    example: Optional[Any] = None
-    examples: Optional[Dict[str, Union[Example, Reference]]] = None
-    encoding: Optional[Dict[str, Encoding]] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:46
+from typing import Any, Dict, Optional, Union
+
+from pydantic import BaseModel, Field
+
+from .encoding import Encoding
+from .example import Example
+from .reference import Reference
+from .schema import Schema
+
+
+class MediaType(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#media-type-object
+    """
+
+    media_type_schema: Optional[Union[Reference, Schema]] = Field(default=None, alias="schema")
+    example: Optional[Any] = None
+    examples: Optional[Dict[str, Union[Example, Reference]]] = None
+    encoding: Optional[Dict[str, Encoding]] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/operation.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/operation.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:48
-from typing import Dict, List, Optional, Union
-
-from pydantic import BaseModel
-
-from .callback import Callback
-from .external_documentation import ExternalDocumentation
-from .parameter import Parameter
-from .reference import Reference
-from .request_body import RequestBody
-from .response import Response
-from .security_requirement import SecurityRequirement
-from .server import Server
-
-
-class Operation(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#operation-object
-    """
-
-    tags: Optional[List[str]] = None
-    summary: Optional[str] = None
-    description: Optional[str] = None
-    externalDocs: Optional[ExternalDocumentation] = None
-    operationId: Optional[str] = None
-    parameters: Optional[List[Parameter]] = None
-    requestBody: Optional[Union[RequestBody, Reference]] = None
-    responses: Optional[Dict[str, Response]] = None
-    callbacks: Optional[Dict[str, Callback]] = None
-
-    deprecated: Optional[bool] = False
-    security: Optional[List[SecurityRequirement]] = None
-    servers: Optional[List[Server]] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:48
+from typing import Dict, List, Optional, Union
+
+from pydantic import BaseModel
+
+from .callback import Callback
+from .external_documentation import ExternalDocumentation
+from .parameter import Parameter
+from .reference import Reference
+from .request_body import RequestBody
+from .response import Response
+from .security_requirement import SecurityRequirement
+from .server import Server
+
+
+class Operation(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#operation-object
+    """
+
+    tags: Optional[List[str]] = None
+    summary: Optional[str] = None
+    description: Optional[str] = None
+    externalDocs: Optional[ExternalDocumentation] = None
+    operationId: Optional[str] = None
+    parameters: Optional[List[Parameter]] = None
+    requestBody: Optional[Union[RequestBody, Reference]] = None
+    responses: Optional[Dict[str, Response]] = None
+    callbacks: Optional[Dict[str, Callback]] = None
+
+    deprecated: Optional[bool] = False
+    security: Optional[List[SecurityRequirement]] = None
+    servers: Optional[List[Server]] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/parameter.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/parameter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:49
-from typing import Any, Dict, Optional, Union
-
-from pydantic import BaseModel, Field
-
-from .example import Example
-from .media_type import MediaType
-from .parameter_in_type import ParameterInType
-from .reference import Reference
-from .schema import Schema
-
-
-class Parameter(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#parameter-object
-    """
-
-    name: str
-    param_in: ParameterInType = Field(alias="in")
-    description: Optional[str] = None
-    required: Optional[bool] = None
-    deprecated: Optional[bool] = None
-    allowEmptyValue: Optional[bool] = None
-    style: Optional[str] = None
-    explode: Optional[bool] = None
-    allowReserved: Optional[bool] = None
-    param_schema: Optional[Union[Reference, Schema]] = Field(default=None, alias="schema")
-    example: Optional[Any] = None
-    examples: Optional[Dict[str, Union[Example, Reference]]] = None
-    content: Optional[Dict[str, MediaType]] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:49
+from typing import Any, Dict, Optional, Union
+
+from pydantic import BaseModel, Field
+
+from .example import Example
+from .media_type import MediaType
+from .parameter_in_type import ParameterInType
+from .reference import Reference
+from .schema import Schema
+
+
+class Parameter(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#parameter-object
+    """
+
+    name: str
+    param_in: ParameterInType = Field(alias="in")
+    description: Optional[str] = None
+    required: Optional[bool] = None
+    deprecated: Optional[bool] = None
+    allowEmptyValue: Optional[bool] = None
+    style: Optional[str] = None
+    explode: Optional[bool] = None
+    allowReserved: Optional[bool] = None
+    param_schema: Optional[Union[Reference, Schema]] = Field(default=None, alias="schema")
+    example: Optional[Any] = None
+    examples: Optional[Dict[str, Union[Example, Reference]]] = None
+    content: Optional[Dict[str, MediaType]] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/path_item.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/path_item.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:50
-import typing
-from typing import List, Optional, Union
-
-from pydantic import BaseModel, Field
-
-from .parameter import Parameter
-from .reference import Reference
-from .server import Server
-
-if typing.TYPE_CHECKING:
-    from .operation import Operation
-
-
-class PathItem(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#path-item-object
-    """
-    ref: Optional[str] = Field(default=None, alias="$ref")
-    summary: Optional[str] = None
-    description: Optional[str] = None
-    get: Optional["Operation"] = None
-    put: Optional["Operation"] = None
-    post: Optional["Operation"] = None
-    delete: Optional["Operation"] = None
-    options: Optional["Operation"] = None
-    head: Optional["Operation"] = None
-    patch: Optional["Operation"] = None
-    trace: Optional["Operation"] = None
-    servers: Optional[List[Server]] = None
-    parameters: Optional[List[Union[Parameter, Reference]]] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:50
+import typing
+from typing import List, Optional, Union
+
+from pydantic import BaseModel, Field
+
+from .parameter import Parameter
+from .reference import Reference
+from .server import Server
+
+if typing.TYPE_CHECKING:
+    from .operation import Operation
+
+
+class PathItem(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#path-item-object
+    """
+    ref: Optional[str] = Field(default=None, alias="$ref")
+    summary: Optional[str] = None
+    description: Optional[str] = None
+    get: Optional["Operation"] = None
+    put: Optional["Operation"] = None
+    post: Optional["Operation"] = None
+    delete: Optional["Operation"] = None
+    options: Optional["Operation"] = None
+    head: Optional["Operation"] = None
+    patch: Optional["Operation"] = None
+    trace: Optional["Operation"] = None
+    servers: Optional[List[Server]] = None
+    parameters: Optional[List[Union[Parameter, Reference]]] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/schema.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/schema.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:55
-from typing import Any, Dict, List, Optional, Union
-
-from pydantic import BaseModel, Field
-
-from .data_type import DataType
-from .discriminator import Discriminator
-from .external_documentation import ExternalDocumentation
-from .reference import Reference
-from .xml import XML
-
-
-class Schema(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#schema-object
-    """
-    ref: Optional[str] = Field(alias="$ref", default=None)
-    title: Optional[str] = None
-    multipleOf: Optional[float] = Field(default=None, gt=0.0)
-    maximum: Optional[float] = None
-    exclusiveMaximum: Optional[float] = None
-    minimum: Optional[float] = None
-    exclusiveMinimum: Optional[float] = None
-    maxLength: Optional[int] = Field(default=None, ge=0)
-    minLength: Optional[int] = Field(default=None, ge=0)
-    pattern: Optional[str] = None
-    maxItems: Optional[int] = Field(default=None, ge=0)
-    minItems: Optional[int] = Field(default=None, ge=0)
-    uniqueItems: Optional[bool] = None
-    maxProperties: Optional[int] = Field(default=None, ge=0)
-    minProperties: Optional[int] = Field(default=None, ge=0)
-    required: Optional[List[str]] = Field(default=None)
-    enum: Union[None, List[Any]] = Field(default=None)
-    type: Optional[DataType] = Field(default=None)
-    allOf: Optional[List[Union[Reference, "Schema"]]] = None
-    oneOf: Optional[List[Union[Reference, "Schema"]]] = None
-    anyOf: Optional[List[Union[Reference, "Schema"]]] = None
-    schema_not: Optional[Union[Reference, "Schema"]] = Field(default=None, alias="not")
-    items: Optional[Union[Reference, "Schema"]] = None
-    properties: Optional[Dict[str, Union[Reference, "Schema"]]] = None
-    additionalProperties: Optional[Union[bool, Reference, "Schema"]] = None
-    description: Optional[str] = None
-    schema_format: Optional[str] = Field(default=None, alias="format")
-    default: Optional[Any] = None
-    nullable: Optional[bool] = None
-    discriminator: Optional[Discriminator] = None
-    readOnly: Optional[bool] = None
-    writeOnly: Optional[bool] = None
-    xml: Optional[XML] = None
-    externalDocs: Optional[ExternalDocumentation] = None
-    example: Optional[Any] = None
-    deprecated: Optional[bool] = None
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:55
+from typing import Any, Dict, List, Optional, Union
+
+from pydantic import BaseModel, Field
+
+from .data_type import DataType
+from .discriminator import Discriminator
+from .external_documentation import ExternalDocumentation
+from .reference import Reference
+from .xml import XML
+
+
+class Schema(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#schema-object
+    """
+    ref: Optional[str] = Field(alias="$ref", default=None)
+    title: Optional[str] = None
+    multipleOf: Optional[float] = Field(default=None, gt=0.0)
+    maximum: Optional[float] = None
+    exclusiveMaximum: Optional[float] = None
+    minimum: Optional[float] = None
+    exclusiveMinimum: Optional[float] = None
+    maxLength: Optional[int] = Field(default=None, ge=0)
+    minLength: Optional[int] = Field(default=None, ge=0)
+    pattern: Optional[str] = None
+    maxItems: Optional[int] = Field(default=None, ge=0)
+    minItems: Optional[int] = Field(default=None, ge=0)
+    uniqueItems: Optional[bool] = None
+    maxProperties: Optional[int] = Field(default=None, ge=0)
+    minProperties: Optional[int] = Field(default=None, ge=0)
+    required: Optional[List[str]] = Field(default=None)
+    enum: Union[None, List[Any]] = Field(default=None)
+    type: Optional[DataType] = Field(default=None)
+    allOf: Optional[List[Union[Reference, "Schema"]]] = None
+    oneOf: Optional[List[Union[Reference, "Schema"]]] = None
+    anyOf: Optional[List[Union[Reference, "Schema"]]] = None
+    schema_not: Optional[Union[Reference, "Schema"]] = Field(default=None, alias="not")
+    items: Optional[Union[Reference, "Schema"]] = None
+    properties: Optional[Dict[str, Union[Reference, "Schema"]]] = None
+    additionalProperties: Optional[Union[bool, Reference, "Schema"]] = None
+    description: Optional[str] = None
+    schema_format: Optional[str] = Field(default=None, alias="format")
+    default: Optional[Any] = None
+    nullable: Optional[bool] = None
+    discriminator: Optional[Discriminator] = None
+    readOnly: Optional[bool] = None
+    writeOnly: Optional[bool] = None
+    xml: Optional[XML] = None
+    externalDocs: Optional[ExternalDocumentation] = None
+    example: Optional[Any] = None
+    deprecated: Optional[bool] = None
```

### Comparing `flask_openapi3-3.1.1/flask_openapi3/models/security_scheme.py` & `flask_openapi3-4.0.0.dev0/flask_openapi3/models/security_scheme.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/4 9:56
-from typing import Optional
-
-from pydantic import BaseModel, Field
-
-from .oauth_flows import OAuthFlows
-from .security_scheme_in_type import SecuritySchemeInType
-
-
-class SecurityScheme(BaseModel):
-    """
-    https://spec.openapis.org/oas/v3.1.0#security-scheme-object
-    """
-
-    type: str
-    description: Optional[str] = None
-    name: Optional[str] = None
-    security_scheme_in: Optional[SecuritySchemeInType] = Field(default=None, alias="in")
-    scheme: Optional[str] = None
-    bearerFormat: Optional[str] = None
-    flows: Optional[OAuthFlows] = None
-    openIdConnectUrl: Optional[str] = None
-
-    model_config = {
-        "extra": "allow"
-    }
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/4 9:56
+from typing import Optional
+
+from pydantic import BaseModel, Field
+
+from .oauth_flows import OAuthFlows
+from .security_scheme_in_type import SecuritySchemeInType
+
+
+class SecurityScheme(BaseModel):
+    """
+    https://spec.openapis.org/oas/v3.1.0#security-scheme-object
+    """
+
+    type: str
+    description: Optional[str] = None
+    name: Optional[str] = None
+    security_scheme_in: Optional[SecuritySchemeInType] = Field(default=None, alias="in")
+    scheme: Optional[str] = None
+    bearerFormat: Optional[str] = None
+    flows: Optional[OAuthFlows] = None
+    openIdConnectUrl: Optional[str] = None
+
+    model_config = {
+        "extra": "allow"
+    }
```

### Comparing `flask_openapi3-3.1.1/tests/test_api_blueprint.py` & `flask_openapi3-4.0.0.dev0/tests/test_api_blueprint.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/5/17 15:25
-
-from typing import Optional
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import APIBlueprint, OpenAPI
-from flask_openapi3 import Tag, Info
-
-info = Info(title='book API', version='1.0.0')
-
-jwt = {
-    "type": "http",
-    "scheme": "bearer",
-    "bearerFormat": "JWT"
-}
-security_schemes = {"jwt": jwt}
-
-app = OpenAPI(__name__, info=info, security_schemes=security_schemes)
-app.config["TESTING"] = True
-
-tag = Tag(name='book', description="Book")
-security = [{"jwt": []}]
-
-
-class Unauthorized(BaseModel):
-    code: int = Field(-1, description="Status Code")
-    message: str = Field("Unauthorized!", description="Exception Information")
-
-
-api = APIBlueprint(
-    '/book',
-    __name__,
-    url_prefix='/api',
-    abp_tags=[tag],
-    abp_security=security,
-    abp_responses={"401": Unauthorized}
-)
-
-try:
-    api.register_api(api)
-except ValueError as e:
-    assert str(e) == "Cannot register a api blueprint on itself"
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-class BookBody(BaseModel):
-    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
-    author: str = Field(None, min_length=2, max_length=4, description='Author')
-
-
-class BookPath(BaseModel):
-    bid: int = Field(..., description='book id')
-
-
-@api.post('/book', doc_ui=False)
-def create_book(body: BookBody):
-    assert body.age == 3
-    return {"code": 0, "message": "ok"}
-
-
-@api.put('/book/<int:bid>', operation_id='update')
-def update_book(path: BookPath, body: BookBody):
-    assert path.bid == 1
-    assert body.age == 3
-    return {"code": 0, "message": "ok"}
-
-
-@api.patch('/book/<int:bid>')
-def update_book1(path: BookPath, body: BookBody):
-    assert path.bid == 1
-    assert body.age == 3
-    return {"code": 0, "message": "ok"}
-
-
-@api.delete('/book/<int:bid>')
-def delete_book(path: BookPath):
-    assert path.bid == 1
-    return {"code": 0, "message": "ok"}
-
-
-# register api
-app.register_api(api)
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json == app.api_doc
-    assert resp.json["paths"]["/api/book/{bid}"]["put"]["operationId"] == "update"
-    assert resp.json["paths"]["/api/book/{bid}"]["delete"]["operationId"] == "_book_book__int_bid__delete"
-
-
-def test_post(client):
-    resp = client.post("/api/book", json={"age": 3})
-    assert resp.status_code == 200
-
-
-def test_put(client):
-    resp = client.put("/api/book/1", json={"age": 3})
-    assert resp.status_code == 200
-
-
-def test_patch(client):
-    resp = client.patch("/api/book/1", json={"age": 3})
-    assert resp.status_code == 200
-
-
-def test_delete(client):
-    resp = client.delete("/api/book/1")
-    assert resp.status_code == 200
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/5/17 15:25
+
+from typing import Optional
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import APIBlueprint, OpenAPI
+from flask_openapi3 import Tag, Info
+
+info = Info(title='book API', version='1.0.0')
+
+jwt = {
+    "type": "http",
+    "scheme": "bearer",
+    "bearerFormat": "JWT"
+}
+security_schemes = {"jwt": jwt}
+
+app = OpenAPI(__name__, info=info, security_schemes=security_schemes)
+app.config["TESTING"] = True
+
+tag = Tag(name='book', description="Book")
+security = [{"jwt": []}]
+
+
+class Unauthorized(BaseModel):
+    code: int = Field(-1, description="Status Code")
+    message: str = Field("Unauthorized!", description="Exception Information")
+
+
+api = APIBlueprint(
+    '/book',
+    __name__,
+    url_prefix='/api',
+    abp_tags=[tag],
+    abp_security=security,
+    abp_responses={"401": Unauthorized}
+)
+
+try:
+    api.register_api(api)
+except ValueError as e:
+    assert str(e) == "Cannot register a api blueprint on itself"
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+class BookBody(BaseModel):
+    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
+    author: str = Field(None, min_length=2, max_length=4, description='Author')
+
+
+class BookPath(BaseModel):
+    bid: int = Field(..., description='book id')
+
+
+@api.post('/book', doc_ui=False)
+def create_book(body: BookBody):
+    assert body.age == 3
+    return {"code": 0, "message": "ok"}
+
+
+@api.put('/book/<int:bid>', operation_id='update')
+def update_book(path: BookPath, body: BookBody):
+    assert path.bid == 1
+    assert body.age == 3
+    return {"code": 0, "message": "ok"}
+
+
+@api.patch('/book/<int:bid>')
+def update_book1(path: BookPath, body: BookBody):
+    assert path.bid == 1
+    assert body.age == 3
+    return {"code": 0, "message": "ok"}
+
+
+@api.delete('/book/<int:bid>')
+def delete_book(path: BookPath):
+    assert path.bid == 1
+    return {"code": 0, "message": "ok"}
+
+
+# register api
+app.register_api(api)
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json == app.api_doc
+    assert resp.json["paths"]["/api/book/{bid}"]["put"]["operationId"] == "update"
+    assert resp.json["paths"]["/api/book/{bid}"]["delete"]["operationId"] == "_book_book__int_bid__delete"
+
+
+def test_post(client):
+    resp = client.post("/api/book", json={"age": 3})
+    assert resp.status_code == 200
+
+
+def test_put(client):
+    resp = client.put("/api/book/1", json={"age": 3})
+    assert resp.status_code == 200
+
+
+def test_patch(client):
+    resp = client.patch("/api/book/1", json={"age": 3})
+    assert resp.status_code == 200
+
+
+def test_delete(client):
+    resp = client.delete("/api/book/1")
+    assert resp.status_code == 200
```

### Comparing `flask_openapi3-3.1.1/tests/test_api_view.py` & `flask_openapi3-4.0.0.dev0/tests/test_api_view.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/11/4 14:41
-
-from typing import Optional
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import APIView
-from flask_openapi3 import OpenAPI, Tag, Info
-
-info = Info(title='book API', version='1.0.0')
-jwt = {
-    "type": "http",
-    "scheme": "bearer",
-    "bearerFormat": "JWT"
-}
-security_schemes = {"jwt": jwt}
-
-app = OpenAPI(__name__, info=info, security_schemes=security_schemes)
-app.config["TESTING"] = True
-security = [{"jwt": []}]
-
-api_view = APIView(url_prefix="/api/v1/<name>", view_tags=[Tag(name="book")], view_security=security)
-
-
-class BookPath(BaseModel):
-    id: int = Field(..., description="book ID")
-    name: str
-
-
-class BookQuery(BaseModel):
-    age: Optional[int] = Field(None, description='Age')
-
-
-class BookBody(BaseModel):
-    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
-    author: str = Field(None, min_length=2, max_length=4, description='Author')
-
-
-@api_view.route("/book")
-class BookListAPIView:
-    a = 1
-
-    @api_view.doc(summary="get book list")
-    def get(self, query: BookQuery):
-        print(self.a)
-        return query.model_dump_json()
-
-    @api_view.doc(summary="create book")
-    def post(self, body: BookBody):
-        """description for a created book"""
-        return body.model_dump_json()
-
-
-@api_view.route("/book/<id>")
-class BookAPIView:
-    @api_view.doc(summary="get book")
-    def get(self, path: BookPath):
-        print(path)
-        return "get"
-
-    @api_view.doc(summary="update book", operation_id="update")
-    def put(self, path: BookPath):
-        print(path)
-        return "put"
-
-    @api_view.doc(summary="delete book", deprecated=True)
-    def delete(self, path: BookPath):
-        print(path)
-        return "delete"
-
-
-app.register_api_view(api_view)
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json == app.api_doc
-    assert resp.json["paths"]["/api/v1/{name}/book/{id}"]["put"]["operationId"] == "update"
-    assert resp.json["paths"]["/api/v1/{name}/book/{id}"]["delete"][
-               "operationId"] == "BookAPIView_delete_book__id__delete"
-
-
-def test_get_list(client):
-    resp = client.get("/api/v1/name1/book")
-    assert resp.status_code == 200
-
-
-def test_post(client):
-    resp = client.post("/api/v1/name1/book", json={"age": 3})
-    assert resp.status_code == 200
-
-
-def test_put(client):
-    resp = client.put("/api/v1/name1/book/1", json={"age": 3})
-    assert resp.status_code == 200
-
-
-def test_get(client):
-    resp = client.get("/api/v1/name1/book/1")
-    assert resp.status_code == 200
-
-
-def test_delete(client):
-    resp = client.delete("/api/v1/name1/book/1")
-    assert resp.status_code == 200
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/11/4 14:41
+
+from typing import Optional
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import APIView
+from flask_openapi3 import OpenAPI, Tag, Info
+
+info = Info(title='book API', version='1.0.0')
+jwt = {
+    "type": "http",
+    "scheme": "bearer",
+    "bearerFormat": "JWT"
+}
+security_schemes = {"jwt": jwt}
+
+app = OpenAPI(__name__, info=info, security_schemes=security_schemes)
+app.config["TESTING"] = True
+security = [{"jwt": []}]
+
+api_view = APIView(url_prefix="/api/v1/<name>", view_tags=[Tag(name="book")], view_security=security)
+
+
+class BookPath(BaseModel):
+    id: int = Field(..., description="book ID")
+    name: str
+
+
+class BookQuery(BaseModel):
+    age: Optional[int] = Field(None, description='Age')
+
+
+class BookBody(BaseModel):
+    age: Optional[int] = Field(..., ge=2, le=4, description='Age')
+    author: str = Field(None, min_length=2, max_length=4, description='Author')
+
+
+@api_view.route("/book")
+class BookListAPIView:
+    a = 1
+
+    @api_view.doc(summary="get book list")
+    def get(self, query: BookQuery):
+        print(self.a)
+        return query.model_dump_json()
+
+    @api_view.doc(summary="create book")
+    def post(self, body: BookBody):
+        """description for a created book"""
+        return body.model_dump_json()
+
+
+@api_view.route("/book/<id>")
+class BookAPIView:
+    @api_view.doc(summary="get book")
+    def get(self, path: BookPath):
+        print(path)
+        return "get"
+
+    @api_view.doc(summary="update book", operation_id="update")
+    def put(self, path: BookPath):
+        print(path)
+        return "put"
+
+    @api_view.doc(summary="delete book", deprecated=True)
+    def delete(self, path: BookPath):
+        print(path)
+        return "delete"
+
+
+app.register_api_view(api_view)
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json == app.api_doc
+    assert resp.json["paths"]["/api/v1/{name}/book/{id}"]["put"]["operationId"] == "update"
+    assert resp.json["paths"]["/api/v1/{name}/book/{id}"]["delete"][
+               "operationId"] == "BookAPIView_delete_book__id__delete"
+
+
+def test_get_list(client):
+    resp = client.get("/api/v1/name1/book")
+    assert resp.status_code == 200
+
+
+def test_post(client):
+    resp = client.post("/api/v1/name1/book", json={"age": 3})
+    assert resp.status_code == 200
+
+
+def test_put(client):
+    resp = client.put("/api/v1/name1/book/1", json={"age": 3})
+    assert resp.status_code == 200
+
+
+def test_get(client):
+    resp = client.get("/api/v1/name1/book/1")
+    assert resp.status_code == 200
+
+
+def test_delete(client):
+    resp = client.delete("/api/v1/name1/book/1")
+    assert resp.status_code == 200
```

### Comparing `flask_openapi3-3.1.1/tests/test_api_view_args.py` & `flask_openapi3-4.0.0.dev0/tests/test_api_view_args.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/11/4 14:41
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import APIView
-from flask_openapi3 import OpenAPI
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-
-api_view = APIView(url_prefix="/api/v1")
-
-
-class BookPath(BaseModel):
-    id: int = Field(..., description="book ID")
-
-
-@api_view.route("/book")
-class BookListAPIView:
-    def __init__(self, view_kwargs=None):
-        self.a = view_kwargs.get("a")
-
-    @api_view.doc(summary="get book list")
-    def get(self):
-        return {"a": self.a}
-
-
-@api_view.route("/book/<id>")
-class BookAPIView:
-    def __init__(self, view_kwargs=None):
-        self.b = view_kwargs.get("b")
-
-    @api_view.doc(summary="get book list")
-    def get(self, path: BookPath):
-        print(path)
-        return {"b": self.b}
-
-
-app.register_api_view(
-    api_view,
-    view_kwargs={
-        "a": 1,
-        "b": 2
-    }
-)
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_get_list_view_kwargs(client):
-    resp = client.get("/api/v1/book")
-    assert resp.status_code == 200
-
-    assert resp.json["a"] == 1
-
-
-def test_get_view_kwargs(client):
-    resp = client.get("/api/v1/book/1")
-    assert resp.status_code == 200
-
-    assert resp.json["b"] == 2
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/11/4 14:41
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import APIView
+from flask_openapi3 import OpenAPI
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+
+api_view = APIView(url_prefix="/api/v1")
+
+
+class BookPath(BaseModel):
+    id: int = Field(..., description="book ID")
+
+
+@api_view.route("/book")
+class BookListAPIView:
+    def __init__(self, view_kwargs=None):
+        self.a = view_kwargs.get("a")
+
+    @api_view.doc(summary="get book list")
+    def get(self):
+        return {"a": self.a}
+
+
+@api_view.route("/book/<id>")
+class BookAPIView:
+    def __init__(self, view_kwargs=None):
+        self.b = view_kwargs.get("b")
+
+    @api_view.doc(summary="get book list")
+    def get(self, path: BookPath):
+        print(path)
+        return {"b": self.b}
+
+
+app.register_api_view(
+    api_view,
+    view_kwargs={
+        "a": 1,
+        "b": 2
+    }
+)
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_get_list_view_kwargs(client):
+    resp = client.get("/api/v1/book")
+    assert resp.status_code == 200
+
+    assert resp.json["a"] == 1
+
+
+def test_get_view_kwargs(client):
+    resp = client.get("/api/v1/book/1")
+    assert resp.status_code == 200
+
+    assert resp.json["b"] == 2
```

### Comparing `flask_openapi3-3.1.1/tests/test_async.py` & `flask_openapi3-4.0.0.dev0/tests/test_async.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/12/5 10:27
-
-from typing import Optional
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import OpenAPI, APIView
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-api_view = APIView(url_prefix="/api/v1")
-
-
-class Query(BaseModel):
-    q: str
-
-
-class BookQuery(BaseModel):
-    age: Optional[int] = Field(None, description="Age")
-
-
-class BookBody(BaseModel):
-    age: Optional[int] = Field(..., ge=2, le=4, description="Age")
-    author: str = Field(None, min_length=2, max_length=4, description="Author")
-
-
-@app.get("/open/api")
-async def get_openapi(query: Query):
-    print(query)
-    return "GET, OpenAPI!"
-
-
-@app.post("/open/api")
-async def post_openapi(body: Query):
-    print(body)
-    return "POST, OpenAPI!"
-
-
-@api_view.route("/book")
-class BookListAPIView:
-
-    @api_view.doc(summary="get book list")
-    async def get(self, query: BookQuery):
-        return query.model_dump_json()
-
-    @api_view.doc(summary="create book")
-    async def post(self, body: BookBody):
-        """description for a created book"""
-        return body.model_dump_json()
-
-
-app.register_api_view(api_view)
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json == app.api_doc
-
-
-def test_get_openapi(client):
-    resp = client.get("/open/api?q=1")
-    assert resp.status_code == 200
-    assert resp.text == "GET, OpenAPI!"
-
-
-def test_post_openapi(client):
-    resp = client.post("/open/api", json={"q": "string"})
-    assert resp.status_code == 200
-    assert resp.text == "POST, OpenAPI!"
-
-
-def test_get_list(client):
-    resp = client.get("/api/v1/book")
-    assert resp.status_code == 200
-
-
-def test_post(client):
-    resp = client.post("/api/v1/book", json={"age": 1})
-    assert resp.status_code == 422
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/12/5 10:27
+
+from typing import Optional
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import OpenAPI, APIView
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+api_view = APIView(url_prefix="/api/v1")
+
+
+class Query(BaseModel):
+    q: str
+
+
+class BookQuery(BaseModel):
+    age: Optional[int] = Field(None, description="Age")
+
+
+class BookBody(BaseModel):
+    age: Optional[int] = Field(..., ge=2, le=4, description="Age")
+    author: str = Field(None, min_length=2, max_length=4, description="Author")
+
+
+@app.get("/open/api")
+async def get_openapi(query: Query):
+    print(query)
+    return "GET, OpenAPI!"
+
+
+@app.post("/open/api")
+async def post_openapi(body: Query):
+    print(body)
+    return "POST, OpenAPI!"
+
+
+@api_view.route("/book")
+class BookListAPIView:
+
+    @api_view.doc(summary="get book list")
+    async def get(self, query: BookQuery):
+        return query.model_dump_json()
+
+    @api_view.doc(summary="create book")
+    async def post(self, body: BookBody):
+        """description for a created book"""
+        return body.model_dump_json()
+
+
+app.register_api_view(api_view)
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json == app.api_doc
+
+
+def test_get_openapi(client):
+    resp = client.get("/open/api?q=1")
+    assert resp.status_code == 200
+    assert resp.text == "GET, OpenAPI!"
+
+
+def test_post_openapi(client):
+    resp = client.post("/open/api", json={"q": "string"})
+    assert resp.status_code == 200
+    assert resp.text == "POST, OpenAPI!"
+
+
+def test_get_list(client):
+    resp = client.get("/api/v1/book")
+    assert resp.status_code == 200
+
+
+def test_post(client):
+    resp = client.post("/api/v1/book", json={"age": 1})
+    assert resp.status_code == 422
```

### Comparing `flask_openapi3-3.1.1/tests/test_empty_body.py` & `flask_openapi3-4.0.0.dev0/tests/test_empty_body.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2021/12/1 9:39
-
-import pytest
-from pydantic import BaseModel
-
-from flask_openapi3 import Info, OpenAPI
-
-info = Info(title='book API', version='1.0.0')
-
-app = OpenAPI(__name__, info=info)
-app.config["TESTING"] = True
-
-
-class CreateBookBody(BaseModel):
-    pass
-
-    model_config = {
-        "extra": "allow",
-    }
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-@app.post('/book')
-def create_book(body: CreateBookBody):
-    print(body.model_dump())
-    return {"code": 0, "message": "ok"}
-
-
-def test_post(client):
-    resp = client.post("/book", json={'aaa': 111, 'bbb': 222})
-    print(resp.json)
-    assert resp.status_code == 200
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2021/12/1 9:39
+
+import pytest
+from pydantic import BaseModel
+
+from flask_openapi3 import Info, OpenAPI
+
+info = Info(title='book API', version='1.0.0')
+
+app = OpenAPI(__name__, info=info)
+app.config["TESTING"] = True
+
+
+class CreateBookBody(BaseModel):
+    pass
+
+    model_config = {
+        "extra": "allow",
+    }
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+@app.post('/book')
+def create_book(body: CreateBookBody):
+    print(body.model_dump())
+    return {"code": 0, "message": "ok"}
+
+
+def test_post(client):
+    resp = client.post("/book", json={'aaa': 111, 'bbb': 222})
+    print(resp.json)
+    assert resp.status_code == 200
```

### Comparing `flask_openapi3-3.1.1/tests/test_enum.py` & `flask_openapi3-4.0.0.dev0/tests/test_enum.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/2/5 14:54
-
-from enum import Enum
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import Info
-from flask_openapi3 import OpenAPI
-
-app = OpenAPI(
-    __name__,
-    info=Info(title='Enum demo', version='1.0.0')
-)
-
-app.config["TESTING"] = True
-
-
-class Language(str, Enum):
-    cn = 'Chinese'
-    en = 'English'
-
-
-class LanguagePath(BaseModel):
-    language: Language = Field(..., description='Language')
-
-
-@app.get('/<language>')
-def get_enum(path: LanguagePath):
-    print(path)
-    return {}
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    _json = resp.json
-    assert resp.status_code == 200
-    assert _json["components"]["schemas"].get("Language") is not None
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/2/5 14:54
+
+from enum import Enum
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import Info
+from flask_openapi3 import OpenAPI
+
+app = OpenAPI(
+    __name__,
+    info=Info(title='Enum demo', version='1.0.0')
+)
+
+app.config["TESTING"] = True
+
+
+class Language(str, Enum):
+    cn = 'Chinese'
+    en = 'English'
+
+
+class LanguagePath(BaseModel):
+    language: Language = Field(..., description='Language')
+
+
+@app.get('/<language>')
+def get_enum(path: LanguagePath):
+    print(path)
+    return {}
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    _json = resp.json
+    assert resp.status_code == 200
+    assert _json["components"]["schemas"].get("Language") is not None
```

### Comparing `flask_openapi3-3.1.1/tests/test_fixed_externaldocs_support.py` & `flask_openapi3-4.0.0.dev0/tests/test_fixed_externaldocs_support.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import pytest
-# from openapi_python_client import GeneratorData, Config
-
-from flask_openapi3 import OpenAPI
-# from flask_openapi3 import ExternalDocumentation
-
-
-@pytest.fixture
-def app():
-    _app = OpenAPI(__name__)
-    _app.config["TESTING"] = True
-    return _app
-
-
-# def test_openapi_api_doc_with_and_without_external_docs(app):
-#     config = Config()
-#
-#     ExternalDocumentation(url="example.com/openapi/markdown", description="Testing the description")
-#
-#     ExternalDocumentation(url="/openapi/markdown", description="Testing the description")
-#
-#     ExternalDocumentation(url="ftp://example.com/openapi/markdown", description="Testing the description")
-#
-#     assert "externalDocs" not in app.api_doc
-#     app.external_docs = ExternalDocumentation(
-#         url="http://example.com/openapi/markdown",
-#         description="Testing the description"
-#     )
-#     assert "externalDocs" in app.api_doc
-#
-#     openapi = GeneratorData.from_dict(data=app.api_doc, config=config)
-#     assert type(openapi) == GeneratorData
-#
-#
-# def test_openapi_api_doc_with_and_without_external_docs_url(app):
-#     client = app.test_client()
-#     config = Config()
-#
-#     resp = client.get("/openapi/openapi.json")
-#     assert resp.status_code == 200
-#     openapi = GeneratorData.from_dict(data=resp.json, config=config)
-#     assert type(openapi) == GeneratorData
-#     assert "externalDocs" not in resp.json
-#
-#     app.external_docs = ExternalDocumentation(
-#         url="http://example.com/openapi/markdown", description="Testing the description")
-#     resp = client.get("/openapi/openapi.json")
-#     assert resp.status_code == 200
-#     openapi = GeneratorData.from_dict(data=resp.json, config=config)
-#     assert type(openapi) == GeneratorData
-#     assert "externalDocs" in resp.json
+import pytest
+# from openapi_python_client import GeneratorData, Config
+
+from flask_openapi3 import OpenAPI
+# from flask_openapi3 import ExternalDocumentation
+
+
+@pytest.fixture
+def app():
+    _app = OpenAPI(__name__)
+    _app.config["TESTING"] = True
+    return _app
+
+
+# def test_openapi_api_doc_with_and_without_external_docs(app):
+#     config = Config()
+#
+#     ExternalDocumentation(url="example.com/openapi/markdown", description="Testing the description")
+#
+#     ExternalDocumentation(url="/openapi/markdown", description="Testing the description")
+#
+#     ExternalDocumentation(url="ftp://example.com/openapi/markdown", description="Testing the description")
+#
+#     assert "externalDocs" not in app.api_doc
+#     app.external_docs = ExternalDocumentation(
+#         url="http://example.com/openapi/markdown",
+#         description="Testing the description"
+#     )
+#     assert "externalDocs" in app.api_doc
+#
+#     openapi = GeneratorData.from_dict(data=app.api_doc, config=config)
+#     assert type(openapi) == GeneratorData
+#
+#
+# def test_openapi_api_doc_with_and_without_external_docs_url(app):
+#     client = app.test_client()
+#     config = Config()
+#
+#     resp = client.get("/openapi/openapi.json")
+#     assert resp.status_code == 200
+#     openapi = GeneratorData.from_dict(data=resp.json, config=config)
+#     assert type(openapi) == GeneratorData
+#     assert "externalDocs" not in resp.json
+#
+#     app.external_docs = ExternalDocumentation(
+#         url="http://example.com/openapi/markdown", description="Testing the description")
+#     resp = client.get("/openapi/openapi.json")
+#     assert resp.status_code == 200
+#     openapi = GeneratorData.from_dict(data=resp.json, config=config)
+#     assert type(openapi) == GeneratorData
+#     assert "externalDocs" in resp.json
```

### Comparing `flask_openapi3-3.1.1/tests/test_multi_decorator.py` & `flask_openapi3-4.0.0.dev0/tests/test_multi_decorator.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/9/7 9:46
-import pytest
-from flask import request
-
-from flask_openapi3 import OpenAPI
-
-app = OpenAPI(__name__)
-
-
-@app.get("/t")
-@app.get("/tt")
-def get_t():
-    return request.url
-
-
-@app.post("/t")
-@app.post("/tt")
-def post_t():
-    return request.url
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_get_t(client):
-    r = client.get("/t")
-    assert r.text == "http://localhost/t"
-    r = client.get("/tt")
-    assert r.text == "http://localhost/tt"
-
-
-def test_post_t(client):
-    r = client.post("/t")
-    assert r.text == "http://localhost/t"
-    r = client.post("/tt")
-    assert r.text == "http://localhost/tt"
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/9/7 9:46
+import pytest
+from flask import request
+
+from flask_openapi3 import OpenAPI
+
+app = OpenAPI(__name__)
+
+
+@app.get("/t")
+@app.get("/tt")
+def get_t():
+    return request.url
+
+
+@app.post("/t")
+@app.post("/tt")
+def post_t():
+    return request.url
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_get_t(client):
+    r = client.get("/t")
+    assert r.text == "http://localhost/t"
+    r = client.get("/tt")
+    assert r.text == "http://localhost/tt"
+
+
+def test_post_t(client):
+    r = client.post("/t")
+    assert r.text == "http://localhost/t"
+    r = client.post("/tt")
+    assert r.text == "http://localhost/tt"
```

### Comparing `flask_openapi3-3.1.1/tests/test_nested_apiblueprint.py` & `flask_openapi3-4.0.0.dev0/tests/test_nested_apiblueprint.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/4/2 9:09
-
-import pytest
-from pydantic import BaseModel
-
-from flask_openapi3 import APIBlueprint, OpenAPI, Tag
-
-app = OpenAPI(__name__)
-
-api = APIBlueprint('book', __name__, url_prefix='/api/book/<name>')
-api_english = APIBlueprint('english', __name__)
-api_chinese = APIBlueprint('chinese', __name__)
-
-
-class BookPath(BaseModel):
-    name: str
-
-
-@api_english.post('/english')
-def create_english_book(path: BookPath):
-    return {"message": "english", "name": path.name}
-
-
-@api_chinese.post('/chinese', tags=[Tag(name="chinese")])
-def create_chinese_book(path: BookPath):
-    return {"message": "chinese", "name": path.name}
-
-
-# register nested api
-api.register_api(api_english)
-api.register_api(api_chinese)
-# register api
-app.register_api(api)
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json == app.api_doc
-
-
-def test_post_english(client):
-    resp = client.post("/api/book/name1/english")
-    assert resp.status_code == 200
-    assert resp.json == {"message": "english", "name": "name1"}
-
-
-def test_post_chinese(client):
-    resp = client.post("/api/book/name2/chinese")
-    assert resp.status_code == 200
-    assert resp.json == {"message": "chinese", "name": "name2"}
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/4/2 9:09
+
+import pytest
+from pydantic import BaseModel
+
+from flask_openapi3 import APIBlueprint, OpenAPI, Tag
+
+app = OpenAPI(__name__)
+
+api = APIBlueprint('book', __name__, url_prefix='/api/book/<name>')
+api_english = APIBlueprint('english', __name__)
+api_chinese = APIBlueprint('chinese', __name__)
+
+
+class BookPath(BaseModel):
+    name: str
+
+
+@api_english.post('/english')
+def create_english_book(path: BookPath):
+    return {"message": "english", "name": path.name}
+
+
+@api_chinese.post('/chinese', tags=[Tag(name="chinese")])
+def create_chinese_book(path: BookPath):
+    return {"message": "chinese", "name": path.name}
+
+
+# register nested api
+api.register_api(api_english)
+api.register_api(api_chinese)
+# register api
+app.register_api(api)
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json == app.api_doc
+
+
+def test_post_english(client):
+    resp = client.post("/api/book/name1/english")
+    assert resp.status_code == 200
+    assert resp.json == {"message": "english", "name": "name1"}
+
+
+def test_post_chinese(client):
+    resp = client.post("/api/book/name2/chinese")
+    assert resp.status_code == 200
+    assert resp.json == {"message": "chinese", "name": "name2"}
```

### Comparing `flask_openapi3-3.1.1/tests/test_options_in_viewfunc.py` & `flask_openapi3-4.0.0.dev0/tests/test_options_in_viewfunc.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/5/15 14:19
-
-import pytest
-
-from flask_openapi3 import APIBlueprint, OpenAPI
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-
-
-def get_operation_id_for_path_callback(*, name: str, path: str, method: str) -> str:
-    print(name, path, method)
-    return name
-
-
-api = APIBlueprint(
-    '/book',
-    __name__,
-    url_prefix='/api',
-    operation_id_callback=get_operation_id_for_path_callback,
-)
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-@app.get('/book', endpoint='endpoint_get_book')
-def get_book():
-    return 'app_book'
-
-
-@api.post('/book', endpoint='endpoint_post_book')
-def create_book():
-    return 'api_book'
-
-
-# register api
-app.register_api(api)
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json == app.api_doc
-    assert resp.json["paths"]["/book"]["get"]["operationId"] == "get_book_book_get"  # Default operation_id generator
-    assert resp.json["paths"]["/api/book"]["post"]["operationId"] == "/book"  # Custom callback operation_id
-
-
-def test_get(client):
-    resp = client.get("/book")
-
-    assert resp.text == 'app_book'
-    assert 'endpoint_get_book' in app.view_functions.keys()
-
-
-def test_post(client):
-    resp = client.post("/api/book")
-
-    assert resp.text == 'api_book'
-    assert '/book.endpoint_post_book' in app.view_functions.keys()
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/5/15 14:19
+
+import pytest
+
+from flask_openapi3 import APIBlueprint, OpenAPI
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+
+
+def get_operation_id_for_path_callback(*, name: str, path: str, method: str) -> str:
+    print(name, path, method)
+    return name
+
+
+api = APIBlueprint(
+    '/book',
+    __name__,
+    url_prefix='/api',
+    operation_id_callback=get_operation_id_for_path_callback,
+)
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+@app.get('/book', endpoint='endpoint_get_book')
+def get_book():
+    return 'app_book'
+
+
+@api.post('/book', endpoint='endpoint_post_book')
+def create_book():
+    return 'api_book'
+
+
+# register api
+app.register_api(api)
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json == app.api_doc
+    assert resp.json["paths"]["/book"]["get"]["operationId"] == "get_book_book_get"  # Default operation_id generator
+    assert resp.json["paths"]["/api/book"]["post"]["operationId"] == "/book"  # Custom callback operation_id
+
+
+def test_get(client):
+    resp = client.get("/book")
+
+    assert resp.text == 'app_book'
+    assert 'endpoint_get_book' in app.view_functions.keys()
+
+
+def test_post(client):
+    resp = client.post("/api/book")
+
+    assert resp.text == 'api_book'
+    assert '/book.endpoint_post_book' in app.view_functions.keys()
```

### Comparing `flask_openapi3-3.1.1/tests/test_pydantic_calculated_fields.py` & `flask_openapi3-4.0.0.dev0/tests/test_pydantic_calculated_fields.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2024/1/28 16:38
-from functools import cached_property
-
-import pytest
-from pydantic import BaseModel, Field, computed_field
-
-from flask_openapi3 import OpenAPI
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-class User(BaseModel):
-    firstName: str = Field(title="First Name")
-    lastName: str
-
-    @computed_field(title="Display Name")
-    @cached_property
-    def display_name(self) -> str:
-        return f"{self.firstName} {self.lastName}"
-
-
-@app.get("/user", responses={200: User})
-def get_book():
-    return "ok"
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    import pprint
-    pprint.pprint(resp.json)
-    assert resp.json["components"]["schemas"]["User"]["properties"].get("display_name") is not None
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2024/1/28 16:38
+from functools import cached_property
+
+import pytest
+from pydantic import BaseModel, Field, computed_field
+
+from flask_openapi3 import OpenAPI
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+class User(BaseModel):
+    firstName: str = Field(title="First Name")
+    lastName: str
+
+    @computed_field(title="Display Name")
+    @cached_property
+    def display_name(self) -> str:
+        return f"{self.firstName} {self.lastName}"
+
+
+@app.get("/user", responses={200: User})
+def get_book():
+    return "ok"
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    import pprint
+    pprint.pprint(resp.json)
+    assert resp.json["components"]["schemas"]["User"]["properties"].get("display_name") is not None
```

### Comparing `flask_openapi3-3.1.1/tests/test_pydantic_custom_root_types.py` & `flask_openapi3-4.0.0.dev0/tests/test_pydantic_custom_root_types.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/2/27 16:53
-from typing import List, Dict, Any
-
-import pytest
-from pydantic import BaseModel, RootModel
-
-from flask_openapi3 import OpenAPI, Tag
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-
-
-class Sellout(BaseModel):
-    a: str
-    b: int
-
-
-class SelloutList(RootModel):
-    root: List[Sellout]
-
-
-class SelloutDict(RootModel):
-    root: Dict[str, Sellout]
-
-
-class SelloutDict2(RootModel):
-    root: Dict[Any, Any]
-
-
-class SelloutDict3(BaseModel):
-    model_config = {
-        "extra": "allow",
-    }
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-@app.post('/api/v1/sellouts',
-          tags=[Tag(name='Sellout', description='Loren.')],
-          responses={'200': SelloutList}
-          )
-def post_sellout(body: SelloutList):
-    print(body)
-    return body.model_dump_json()
-
-
-@app.post('/api/v2/sellouts',
-          tags=[Tag(name='Sellout', description='Loren.')],
-          responses={'200': SelloutDict}
-          )
-def post_sellout2(body: SelloutDict):
-    print(body)
-    return body.model_dump_json()
-
-
-@app.post('/api/v3/sellouts',
-          tags=[Tag(name='Sellout', description='Loren.')]
-          )
-def post_sellout3(body: SelloutDict2):
-    print(body)
-    return body.model_dump_json()
-
-
-@app.post('/api/v4/sellouts',
-          tags=[Tag(name='Sellout', description='Loren.')]
-          )
-def post_sellout4(body: SelloutDict3):
-    print(body)
-    return body.model_dump_json()
-
-
-def test_v1_sellouts(client):
-    resp = client.post("/api/v1/sellouts", json=[{"a": "string", "b": 0}])
-    assert resp.status_code == 200
-
-
-def test_v2_sellouts(client):
-    resp = client.post("/api/v2/sellouts", json={"additionalProp1": {"a": "string", "b": 0}})
-    assert resp.status_code == 200
-
-
-def test_v3_sellouts(client):
-    resp = client.post("/api/v3/sellouts", json={"a": 11, "b": 23, "c": {"cc": 33, "ccc": 333}})
-    assert resp.status_code == 200
-
-
-def test_v4_sellouts(client):
-    resp = client.post("/api/v4/sellouts", json={"a": 11, "b": 23, "c": {"cc": 33, "ccc": 333}})
-    assert resp.status_code == 200
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/2/27 16:53
+from typing import List, Dict, Any
+
+import pytest
+from pydantic import BaseModel, RootModel
+
+from flask_openapi3 import OpenAPI, Tag
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+
+
+class Sellout(BaseModel):
+    a: str
+    b: int
+
+
+class SelloutList(RootModel):
+    root: List[Sellout]
+
+
+class SelloutDict(RootModel):
+    root: Dict[str, Sellout]
+
+
+class SelloutDict2(RootModel):
+    root: Dict[Any, Any]
+
+
+class SelloutDict3(BaseModel):
+    model_config = {
+        "extra": "allow",
+    }
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+@app.post('/api/v1/sellouts',
+          tags=[Tag(name='Sellout', description='Loren.')],
+          responses={'200': SelloutList}
+          )
+def post_sellout(body: SelloutList):
+    print(body)
+    return body.model_dump_json()
+
+
+@app.post('/api/v2/sellouts',
+          tags=[Tag(name='Sellout', description='Loren.')],
+          responses={'200': SelloutDict}
+          )
+def post_sellout2(body: SelloutDict):
+    print(body)
+    return body.model_dump_json()
+
+
+@app.post('/api/v3/sellouts',
+          tags=[Tag(name='Sellout', description='Loren.')]
+          )
+def post_sellout3(body: SelloutDict2):
+    print(body)
+    return body.model_dump_json()
+
+
+@app.post('/api/v4/sellouts',
+          tags=[Tag(name='Sellout', description='Loren.')]
+          )
+def post_sellout4(body: SelloutDict3):
+    print(body)
+    return body.model_dump_json()
+
+
+def test_v1_sellouts(client):
+    resp = client.post("/api/v1/sellouts", json=[{"a": "string", "b": 0}])
+    assert resp.status_code == 200
+
+
+def test_v2_sellouts(client):
+    resp = client.post("/api/v2/sellouts", json={"additionalProp1": {"a": "string", "b": 0}})
+    assert resp.status_code == 200
+
+
+def test_v3_sellouts(client):
+    resp = client.post("/api/v3/sellouts", json={"a": 11, "b": 23, "c": {"cc": 33, "ccc": 333}})
+    assert resp.status_code == 200
+
+
+def test_v4_sellouts(client):
+    resp = client.post("/api/v4/sellouts", json={"a": 11, "b": 23, "c": {"cc": 33, "ccc": 333}})
+    assert resp.status_code == 200
```

### Comparing `flask_openapi3-3.1.1/tests/test_request.py` & `flask_openapi3-4.0.0.dev0/tests/test_request.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/9/2 15:35
-from functools import wraps
-from typing import List, Optional
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import OpenAPI, FileStorage, RawModel
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-class BookForm(BaseModel):
-    file: FileStorage
-    files: List[FileStorage]
-    string: str
-    string_list: List[str]
-
-
-class BookQuery(BaseModel):
-    age: List[int]
-
-
-class BookBody(BaseModel):
-    age: int
-
-
-class BookCookie(BaseModel):
-    token: Optional[str] = None
-
-
-class BookHeader(BaseModel):
-    Hello1: str = Field("what's up", max_length=12, description="sds")
-    # required
-    hello2: str = Field(..., max_length=12, description="sds")
-    api_key: str = Field(..., description="API Key")
-    x_hello: str = Field(..., max_length=12, description='Header with alias to support dash', alias="x-hello")
-
-
-def decorator(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-@app.get("/query")
-@decorator
-def api_query(query: BookQuery):
-    print(query)
-    return {"code": 0, "message": "ok"}
-
-
-@app.post("/form")
-def api_form(form: BookForm):
-    print(form)
-    return {"code": 0, "message": "ok"}
-
-
-@app.post("/body")
-def api_error_json(body: BookBody):
-    print(body)
-    return {"code": 0, "message": "ok"}
-
-
-@app.get("/header")
-def get_book(header: BookHeader):
-    return header.model_dump(by_alias=True)
-
-
-@app.post("/cookie")
-def api_cookie(cookie: BookCookie):
-    print(cookie)
-    return {"code": 0, "message": "ok"}
-
-
-class BookRaw(RawModel):
-    mimetypes = ["text/csv", "application/json"]
-
-
-@app.post("/raw")
-def api_raw(raw: BookRaw):
-    # raw equals to flask.request
-    assert raw.data == b"raw"
-    assert raw.mimetype == "text/plain"
-    return "ok"
-
-
-def test_query(client):
-    r = client.get("/query")
-    print(r.json)
-    assert r.status_code == 200
-
-
-def test_form(client):
-    from io import BytesIO
-    data = {
-        "file": (BytesIO(b"post-data"), "filename"),
-        "files": [(BytesIO(b"post-data"), "filename"), (BytesIO(b"post-data"), "filename")],
-        "string": "a",
-        "string_list": ["a", "b", "c"]
-    }
-    r = client.post("/form", data=data, content_type="multipart/form-data")
-    assert r.status_code == 200
-
-
-def test_error_json(client):
-    r = client.post("/body", json="{age: 1}")
-    assert r.status_code == 422
-
-
-def test_cookie(client):
-    r = client.post("/cookie")
-    print(r.json)
-    assert r.status_code == 200
-
-
-def test_header(client):
-    headers = {"Hello1": "111", "hello2": "222", "api_key": "333", "x-hello": "444"}
-    resp = client.get("/header", headers=headers)
-    print(resp.json)
-    assert resp.status_code == 200
-    assert resp.json == headers
-
-
-def test_raw(client):
-    resp = client.post("/raw", data="raw", headers={"Content-Type": "text/plain"})
-    assert resp.status_code == 200
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/9/2 15:35
+from functools import wraps
+from typing import List, Optional
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import OpenAPI, FileStorage, RawModel
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+class BookForm(BaseModel):
+    file: FileStorage
+    files: List[FileStorage]
+    string: str
+    string_list: List[str]
+
+
+class BookQuery(BaseModel):
+    age: List[int]
+
+
+class BookBody(BaseModel):
+    age: int
+
+
+class BookCookie(BaseModel):
+    token: Optional[str] = None
+
+
+class BookHeader(BaseModel):
+    Hello1: str = Field("what's up", max_length=12, description="sds")
+    # required
+    hello2: str = Field(..., max_length=12, description="sds")
+    api_key: str = Field(..., description="API Key")
+    x_hello: str = Field(..., max_length=12, description='Header with alias to support dash', alias="x-hello")
+
+
+def decorator(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+@app.get("/query")
+@decorator
+def api_query(query: BookQuery):
+    print(query)
+    return {"code": 0, "message": "ok"}
+
+
+@app.post("/form")
+def api_form(form: BookForm):
+    print(form)
+    return {"code": 0, "message": "ok"}
+
+
+@app.post("/body")
+def api_error_json(body: BookBody):
+    print(body)
+    return {"code": 0, "message": "ok"}
+
+
+@app.get("/header")
+def get_book(header: BookHeader):
+    return header.model_dump(by_alias=True)
+
+
+@app.post("/cookie")
+def api_cookie(cookie: BookCookie):
+    print(cookie)
+    return {"code": 0, "message": "ok"}
+
+
+class BookRaw(RawModel):
+    mimetypes = ["text/csv", "application/json"]
+
+
+@app.post("/raw")
+def api_raw(raw: BookRaw):
+    # raw equals to flask.request
+    assert raw.data == b"raw"
+    assert raw.mimetype == "text/plain"
+    return "ok"
+
+
+def test_query(client):
+    r = client.get("/query")
+    print(r.json)
+    assert r.status_code == 200
+
+
+def test_form(client):
+    from io import BytesIO
+    data = {
+        "file": (BytesIO(b"post-data"), "filename"),
+        "files": [(BytesIO(b"post-data"), "filename"), (BytesIO(b"post-data"), "filename")],
+        "string": "a",
+        "string_list": ["a", "b", "c"]
+    }
+    r = client.post("/form", data=data, content_type="multipart/form-data")
+    assert r.status_code == 200
+
+
+def test_error_json(client):
+    r = client.post("/body", json="{age: 1}")
+    assert r.status_code == 422
+
+
+def test_cookie(client):
+    r = client.post("/cookie")
+    print(r.json)
+    assert r.status_code == 200
+
+
+def test_header(client):
+    headers = {"Hello1": "111", "hello2": "222", "api_key": "333", "x-hello": "444"}
+    resp = client.get("/header", headers=headers)
+    print(resp.json)
+    assert resp.status_code == 200
+    assert resp.json == headers
+
+
+def test_raw(client):
+    resp = client.post("/raw", data="raw", headers={"Content-Type": "text/plain"})
+    assert resp.status_code == 200
```

### Comparing `flask_openapi3-3.1.1/tests/test_response.py` & `flask_openapi3-4.0.0.dev0/tests/test_response.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/9 11:23
-from http import HTTPStatus
-
-import pytest
-from pydantic import BaseModel, Field
-
-from flask_openapi3 import OpenAPI, APIBlueprint
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-api = APIBlueprint("/api", __name__, url_prefix="/api")
-
-
-class BookResponse(BaseModel):
-    code: int = Field(0, description="Status Code")
-    message: str = Field("ok", description="Exception Information")
-
-
-class BookPath(BaseModel):
-    bid: int = Field(..., description="book id")
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-@app.get(
-    "/book/<int:bid>",
-    responses={
-        HTTPStatus.OK: BookResponse,
-        "201": BookResponse,
-        202: {"content": {"text/html": {"schema": {"type": "string"}}}},
-        204: None
-    }
-)
-def get_book(path: BookPath):
-    print(path)
-    return {"code": 0, "message": "ok"}
-
-
-@api.get("/book", responses={HTTPStatus.OK: BookResponse, "201": BookResponse, 204: None})
-def get_api_book():
-    return {"code": 0, "message": "ok"}
-
-
-app.register_api(api)
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    _json = resp.json
-    assert resp.status_code == 200
-    assert _json["paths"]["/book/{bid}"]["get"]["responses"].keys() - ["200", "201", "202", "204"] == {"422"}
-    assert _json["paths"]["/api/book"]["get"]["responses"].keys() - ["200", "201", "202", "204"] == set()
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/9 11:23
+from http import HTTPStatus
+
+import pytest
+from pydantic import BaseModel, Field
+
+from flask_openapi3 import OpenAPI, APIBlueprint
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+api = APIBlueprint("/api", __name__, url_prefix="/api")
+
+
+class BookResponse(BaseModel):
+    code: int = Field(0, description="Status Code")
+    message: str = Field("ok", description="Exception Information")
+
+
+class BookPath(BaseModel):
+    bid: int = Field(..., description="book id")
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+@app.get(
+    "/book/<int:bid>",
+    responses={
+        HTTPStatus.OK: BookResponse,
+        "201": BookResponse,
+        202: {"content": {"text/html": {"schema": {"type": "string"}}}},
+        204: None
+    }
+)
+def get_book(path: BookPath):
+    print(path)
+    return {"code": 0, "message": "ok"}
+
+
+@api.get("/book", responses={HTTPStatus.OK: BookResponse, "201": BookResponse, 204: None})
+def get_api_book():
+    return {"code": 0, "message": "ok"}
+
+
+app.register_api(api)
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    _json = resp.json
+    assert resp.status_code == 200
+    assert _json["paths"]["/book/{bid}"]["get"]["responses"].keys() - ["200", "201", "202", "204"] == {"422"}
+    assert _json["paths"]["/api/book"]["get"]["responses"].keys() - ["200", "201", "202", "204"] == set()
```

### Comparing `flask_openapi3-3.1.1/tests/test_str_body.py` & `flask_openapi3-4.0.0.dev0/tests/test_str_body.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/5/22 8:05
-
-import pytest
-from pydantic import BaseModel
-
-from flask_openapi3 import OpenAPI
-
-app = OpenAPI(__name__)
-app.config["TESTING"] = True
-
-
-class MyModel(BaseModel):
-    text: str
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-@app.post('/path/')
-def create_book1(body: MyModel):
-    return body.text
-
-
-def test_post(client):
-    my_model = MyModel(text='1')
-    resp = client.post("/path/", json=my_model.model_dump_json())
-    assert resp.status_code == 200
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/5/22 8:05
+
+import pytest
+from pydantic import BaseModel
+
+from flask_openapi3 import OpenAPI
+
+app = OpenAPI(__name__)
+app.config["TESTING"] = True
+
+
+class MyModel(BaseModel):
+    text: str
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+@app.post('/path/')
+def create_book1(body: MyModel):
+    return body.text
+
+
+def test_post(client):
+    my_model = MyModel(text='1')
+    resp = client.post("/path/", json=my_model.model_dump_json())
+    assert resp.status_code == 200
```

### Comparing `flask_openapi3-3.1.1/tests/test_swagger_config.py` & `flask_openapi3-4.0.0.dev0/tests/test_swagger_config.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2024/3/10 14:48
-import pytest
-
-from flask_openapi3 import OpenAPI
-
-app = OpenAPI(__name__, swagger_config={"validatorUrl": "https://www.b.com"})
-app.config["TESTING"] = True
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json == app.api_doc
-
-
-def test_swagger(client):
-    resp = client.get("/openapi/swagger")
-    assert resp.status_code == 200
-    assert "https://www.b.com" in resp.text
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2024/3/10 14:48
+import pytest
+
+from flask_openapi3 import OpenAPI
+
+app = OpenAPI(__name__, swagger_config={"validatorUrl": "https://www.b.com"})
+app.config["TESTING"] = True
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json == app.api_doc
+
+
+def test_swagger(client):
+    resp = client.get("/openapi/swagger")
+    assert resp.status_code == 200
+    assert "https://www.b.com" in resp.text
```

### Comparing `flask_openapi3-3.1.1/tests/test_tags.py` & `flask_openapi3-4.0.0.dev0/tests/test_tags.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/12/19 10:34
-
-import pytest
-
-from flask_openapi3 import Info, Tag
-from flask_openapi3 import OpenAPI, APIBlueprint
-
-info = Info(title="book API", version="1.0.0")
-
-app = OpenAPI(__name__, info=info)
-app.config["TESTING"] = True
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-    return client
-
-
-api1 = APIBlueprint("book1", __name__)
-
-
-@api1.get('/book', tags=[Tag(name="book")])
-def get_book():
-    return {"code": 0, "message": "ok"}
-
-
-api2 = APIBlueprint("book2", __name__)
-
-
-@api2.get('/book2', tags=[Tag(name="book")])
-def get_book2():
-    return {"code": 0, "message": "ok"}
-
-
-app.register_api(api1)
-app.register_api(api2)
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    _json = resp.json
-    assert resp.status_code == 200
-    tags = _json["tags"]
-    news_tags = []
-    for tag in tags:
-        if tag not in news_tags:
-            news_tags.append(tag)
-    assert news_tags == tags
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/12/19 10:34
+
+import pytest
+
+from flask_openapi3 import Info, Tag
+from flask_openapi3 import OpenAPI, APIBlueprint
+
+info = Info(title="book API", version="1.0.0")
+
+app = OpenAPI(__name__, info=info)
+app.config["TESTING"] = True
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+    return client
+
+
+api1 = APIBlueprint("book1", __name__)
+
+
+@api1.get('/book', tags=[Tag(name="book")])
+def get_book():
+    return {"code": 0, "message": "ok"}
+
+
+api2 = APIBlueprint("book2", __name__)
+
+
+@api2.get('/book2', tags=[Tag(name="book")])
+def get_book2():
+    return {"code": 0, "message": "ok"}
+
+
+app.register_api(api1)
+app.register_api(api2)
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    _json = resp.json
+    assert resp.status_code == 200
+    tags = _json["tags"]
+    news_tags = []
+    for tag in tags:
+        if tag not in news_tags:
+            news_tags.append(tag)
+    assert news_tags == tags
```

### Comparing `flask_openapi3-3.1.1/tests/test_trail_slash.py` & `flask_openapi3-4.0.0.dev0/tests/test_trail_slash.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2022/5/5 13:28
-
-import pytest
-
-from flask_openapi3 import Info
-from flask_openapi3 import OpenAPI, APIBlueprint
-
-info = Info(title='book API', version='1.0.0')
-
-app = OpenAPI(__name__, info=info)
-app.config["TESTING"] = True
-
-api1 = APIBlueprint('book1', __name__, url_prefix='/api/v1/book1')
-api2 = APIBlueprint('book2', __name__, url_prefix='/api/v1/book2')
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-
-    return client
-
-
-@api1.get('/')
-def get_book():
-    return 'with slash'
-
-
-@api2.get('')
-def get_book2():
-    return 'without slash'
-
-
-app.register_api(api1)
-app.register_api(api2)
-
-
-def test_with_slash1(client):
-    resp = client.get("/api/v1/book1/")
-    assert resp.status_code == 200
-
-
-def test_with_slash2(client):
-    resp = client.get("/api/v1/book1")
-    assert resp.status_code == 308
-
-
-def test_without_slash1(client):
-    resp = client.get("/api/v1/book2/")
-    assert resp.status_code == 404
-
-
-def test_without_slash2(client):
-    resp = client.get("/api/v1/book2")
-    assert resp.status_code == 200
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    _json = resp.json
-    assert _json['paths'].get('/api/v1/book1/') is not None
-    assert _json['paths'].get('/api/v1/book2') is not None
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2022/5/5 13:28
+
+import pytest
+
+from flask_openapi3 import Info
+from flask_openapi3 import OpenAPI, APIBlueprint
+
+info = Info(title='book API', version='1.0.0')
+
+app = OpenAPI(__name__, info=info)
+app.config["TESTING"] = True
+
+api1 = APIBlueprint('book1', __name__, url_prefix='/api/v1/book1')
+api2 = APIBlueprint('book2', __name__, url_prefix='/api/v1/book2')
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+
+    return client
+
+
+@api1.get('/')
+def get_book():
+    return 'with slash'
+
+
+@api2.get('')
+def get_book2():
+    return 'without slash'
+
+
+app.register_api(api1)
+app.register_api(api2)
+
+
+def test_with_slash1(client):
+    resp = client.get("/api/v1/book1/")
+    assert resp.status_code == 200
+
+
+def test_with_slash2(client):
+    resp = client.get("/api/v1/book1")
+    assert resp.status_code == 308
+
+
+def test_without_slash1(client):
+    resp = client.get("/api/v1/book2/")
+    assert resp.status_code == 404
+
+
+def test_without_slash2(client):
+    resp = client.get("/api/v1/book2")
+    assert resp.status_code == 200
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    _json = resp.json
+    assert _json['paths'].get('/api/v1/book1/') is not None
+    assert _json['paths'].get('/api/v1/book2') is not None
```

### Comparing `flask_openapi3-3.1.1/tests/test_validation_error.py` & `flask_openapi3-4.0.0.dev0/tests/test_validation_error.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# -*- coding: utf-8 -*-
-# @Author  : llc
-# @Time    : 2023/7/21 10:32
-from typing import List
-
-import pytest
-from flask import make_response, current_app
-from pydantic import BaseModel, Field, ValidationError
-
-from flask_openapi3 import OpenAPI
-
-
-class GenericTracebackError(BaseModel):
-    location: str = Field(..., example="GenericError.py")
-    line: int = Field(..., example=1)
-    method: str = Field(..., example="GenericError")
-    message: str = Field(..., example="400:Bad Request")
-
-
-class ValidationErrorModel(BaseModel):
-    code: str
-    message: str
-    more_info: List[GenericTracebackError] = Field(..., example=[GenericTracebackError(
-        location="GenericError.py",
-        line=1,
-        method="GenericError",
-        message="400:Bad Request")])
-
-
-def validation_error_callback(e: ValidationError):
-    validation_error_object = ValidationErrorModel(
-        code="400",
-        message=e.json(),
-        more_info=[GenericTracebackError(
-            location="GenericError.py",
-            line=1,
-            method="GenericError",
-            message="400:Bad Request"
-        )]
-    )
-    response = make_response(validation_error_object.model_dump_json())
-    response.headers["Content-Type"] = "application/json"
-    response.status_code = getattr(current_app, "validation_error_status", 422)
-    return response
-
-
-app = OpenAPI(
-    __name__,
-    validation_error_status=400,
-    validation_error_model=ValidationErrorModel,
-    validation_error_callback=validation_error_callback
-)
-app.config["TESTING"] = True
-
-
-@pytest.fixture
-def client():
-    client = app.test_client()
-    return client
-
-
-class BookQuery(BaseModel):
-    age: int = Field(None, description="Age")
-
-
-@app.get("/query")
-def api_query(query: BookQuery):
-    print(query)
-    return {"code": 0, "message": "ok"}
-
-
-def test_openapi(client):
-    resp = client.get("/openapi/openapi.json")
-    assert resp.status_code == 200
-    assert resp.json["components"]["schemas"].get("GenericTracebackError") is not None
-
-
-def test_api_query(client):
-    resp = client.get("/query?age=abc")
-    print(resp.json)
-    assert resp.status_code == 400
+# -*- coding: utf-8 -*-
+# @Author  : llc
+# @Time    : 2023/7/21 10:32
+from typing import List
+
+import pytest
+from flask import make_response, current_app
+from pydantic import BaseModel, Field, ValidationError
+
+from flask_openapi3 import OpenAPI
+
+
+class GenericTracebackError(BaseModel):
+    location: str = Field(..., example="GenericError.py")
+    line: int = Field(..., example=1)
+    method: str = Field(..., example="GenericError")
+    message: str = Field(..., example="400:Bad Request")
+
+
+class ValidationErrorModel(BaseModel):
+    code: str
+    message: str
+    more_info: List[GenericTracebackError] = Field(..., example=[GenericTracebackError(
+        location="GenericError.py",
+        line=1,
+        method="GenericError",
+        message="400:Bad Request")])
+
+
+def validation_error_callback(e: ValidationError):
+    validation_error_object = ValidationErrorModel(
+        code="400",
+        message=e.json(),
+        more_info=[GenericTracebackError(
+            location="GenericError.py",
+            line=1,
+            method="GenericError",
+            message="400:Bad Request"
+        )]
+    )
+    response = make_response(validation_error_object.model_dump_json())
+    response.headers["Content-Type"] = "application/json"
+    response.status_code = getattr(current_app, "validation_error_status", 422)
+    return response
+
+
+app = OpenAPI(
+    __name__,
+    validation_error_status=400,
+    validation_error_model=ValidationErrorModel,
+    validation_error_callback=validation_error_callback
+)
+app.config["TESTING"] = True
+
+
+@pytest.fixture
+def client():
+    client = app.test_client()
+    return client
+
+
+class BookQuery(BaseModel):
+    age: int = Field(None, description="Age")
+
+
+@app.get("/query")
+def api_query(query: BookQuery):
+    print(query)
+    return {"code": 0, "message": "ok"}
+
+
+def test_openapi(client):
+    resp = client.get("/openapi/openapi.json")
+    assert resp.status_code == 200
+    assert resp.json["components"]["schemas"].get("GenericTracebackError") is not None
+
+
+def test_api_query(client):
+    resp = client.get("/query?age=abc")
+    print(resp.json)
+    assert resp.status_code == 400
```

### Comparing `flask_openapi3-3.1.1/.gitignore` & `flask_openapi3-4.0.0.dev0/.gitignore`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-### Python template
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
+### Python template
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
 .idea
```

### Comparing `flask_openapi3-3.1.1/README.md` & `flask_openapi3-4.0.0.dev0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,408 +1,444 @@
 00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
-00000020: 3d22 6874 7470 733a 2f2f 6c75 6f6c 696e  ="https://luolin
-00000030: 6763 6875 6e2e 6769 7468 7562 2e69 6f2f  gchun.github.io/
-00000040: 666c 6173 6b2d 6f70 656e 6170 6933 2f22  flask-openapi3/"
-00000050: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000060: 3e0a 2020 2020 2020 2020 3c69 6d67 2063  >.        <img c
-00000070: 6c61 7373 3d22 6f66 662d 676c 6222 2073  lass="off-glb" s
-00000080: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00000090: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000000a0: 742e 636f 6d2f 6c75 6f6c 696e 6763 6875  t.com/luolingchu
-000000b0: 6e2f 666c 6173 6b2d 6f70 656e 6170 6933  n/flask-openapi3
-000000c0: 2f6d 6173 7465 722f 646f 6373 2f69 6d61  /master/docs/ima
-000000d0: 6765 732f 6c6f 676f 2d74 6578 742e 7376  ges/logo-text.sv
-000000e0: 6722 200a 2020 2020 2020 2020 2020 2020  g" .            
-000000f0: 2077 6964 7468 3d22 3630 2522 2068 6569   width="60%" hei
-00000100: 6768 743d 2261 7574 6f22 2061 6c74 3d22  ght="auto" alt="
-00000110: 6c6f 676f 223e 0a20 2020 203c 2f61 3e0a  logo">.    </a>.
-00000120: 3c2f 6469 763e 0a3c 7020 616c 6967 6e3d  </div>.<p align=
-00000130: 2263 656e 7465 7222 3e0a 2020 2020 3c65  "center">.    <e
-00000140: 6d3e 4765 6e65 7261 7465 2052 4553 5420  m>Generate REST 
-00000150: 4150 4920 616e 6420 4f70 656e 4150 4920  API and OpenAPI 
-00000160: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
-00000170: 7220 796f 7572 2046 6c61 736b 2070 726f  r your Flask pro
-00000180: 6a65 6374 2e3c 2f65 6d3e 0a3c 2f70 3e0a  ject.</em>.</p>.
-00000190: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-000001a0: 223e 0a20 2020 203c 6120 6872 6566 3d22  ">.    <a href="
-000001b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001c0: 6f6d 2f6c 756f 6c69 6e67 6368 756e 2f66  om/luolingchun/f
-000001d0: 6c61 736b 2d6f 7065 6e61 7069 332f 6163  lask-openapi3/ac
-000001e0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000001f0: 7465 7374 732e 796d 6c22 2074 6172 6765  tests.yml" targe
-00000200: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
-00000210: 2020 2020 3c69 6d67 2063 6c61 7373 3d22      <img class="
-00000220: 6f66 662d 676c 6222 2073 7263 3d22 6874  off-glb" src="ht
-00000230: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000240: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
-00000250: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
-00000260: 7475 732f 6c75 6f6c 696e 6763 6875 6e2f  tus/luolingchun/
-00000270: 666c 6173 6b2d 6f70 656e 6170 6933 2f74  flask-openapi3/t
-00000280: 6573 7473 2e79 6d6c 3f62 7261 6e63 683d  ests.yml?branch=
-00000290: 6d61 7374 6572 2220 616c 743d 2274 6573  master" alt="tes
-000002a0: 7422 3e0a 2020 2020 3c2f 613e 0a20 2020  t">.    </a>.   
-000002b0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000002c0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000002d0: 6374 2f66 6c61 736b 2d6f 7065 6e61 7069  ct/flask-openapi
-000002e0: 332f 2220 7461 7267 6574 3d22 5f62 6c61  3/" target="_bla
-000002f0: 6e6b 223e 0a20 2020 2020 2020 203c 696d  nk">.        <im
-00000300: 6720 636c 6173 733d 226f 6666 2d67 6c62  g class="off-glb
-00000310: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000320: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000330: 7069 2f76 2f66 6c61 736b 2d6f 7065 6e61  pi/v/flask-opena
-00000340: 7069 3322 2061 6c74 3d22 7079 7069 223e  pi3" alt="pypi">
-00000350: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
-00000360: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-00000370: 7970 6973 7461 7473 2e6f 7267 2f70 6163  ypistats.org/pac
-00000380: 6b61 6765 732f 666c 6173 6b2d 6f70 656e  kages/flask-open
-00000390: 6170 6933 2220 7461 7267 6574 3d22 5f62  api3" target="_b
-000003a0: 6c61 6e6b 223e 0a20 2020 2020 2020 203c  lank">.        <
-000003b0: 696d 6720 636c 6173 733d 226f 6666 2d67  img class="off-g
-000003c0: 6c62 2220 7372 633d 2268 7474 7073 3a2f  lb" src="https:/
-000003d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000003e0: 7079 7069 2f64 6d2f 666c 6173 6b2d 6f70  pypi/dm/flask-op
-000003f0: 656e 6170 6933 2220 616c 743d 2270 7970  enapi3" alt="pyp
-00000400: 6973 7461 7473 223e 0a20 2020 203c 2f61  istats">.    </a
-00000410: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
-00000420: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000430: 7072 6f6a 6563 742f 666c 6173 6b2d 6f70  project/flask-op
-00000440: 656e 6170 6933 2f22 2074 6172 6765 743d  enapi3/" target=
-00000450: 225f 626c 616e 6b22 3e0a 2020 2020 2020  "_blank">.      
-00000460: 2020 3c69 6d67 2063 6c61 7373 3d22 6f66    <img class="of
-00000470: 662d 676c 6222 2073 7263 3d22 6874 7470  f-glb" src="http
-00000480: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000490: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
-000004a0: 6e73 2f66 6c61 736b 2d6f 7065 6e61 7069  ns/flask-openapi
-000004b0: 3322 2061 6c74 3d22 7079 7069 2076 6572  3" alt="pypi ver
-000004c0: 7369 6f6e 7322 3e0a 2020 2020 3c2f 613e  sions">.    </a>
-000004d0: 0a3c 2f70 3e0a 0a2a 2a46 6c61 736b 204f  .</p>..**Flask O
-000004e0: 7065 6e41 5049 332a 2a20 6973 2061 2077  penAPI3** is a w
-000004f0: 6562 2041 5049 2066 7261 6d65 776f 726b  eb API framework
-00000500: 2062 6173 6564 206f 6e20 2a2a 466c 6173   based on **Flas
-00000510: 6b2a 2a2e 2049 7420 7573 6573 202a 2a50  k**. It uses **P
-00000520: 7964 616e 7469 632a 2a20 746f 2076 6572  ydantic** to ver
-00000530: 6966 7920 6461 7461 2061 6e64 2061 7574  ify data and aut
-00000540: 6f6d 6174 6963 0a67 656e 6572 6174 696f  omatic.generatio
-00000550: 6e20 6f66 2069 6e74 6572 6163 7469 6f6e  n of interaction
-00000560: 2064 6f63 756d 656e 7461 7469 6f6e 3a20   documentation: 
-00000570: 2a2a 5377 6167 6765 722a 2a2c 202a 2a52  **Swagger**, **R
-00000580: 6544 6f63 2a2a 2061 6e64 202a 2a52 6170  eDoc** and **Rap
-00000590: 6944 6f63 2a2a 2e0a 0a54 6865 206b 6579  iDoc**...The key
-000005a0: 2066 6561 7475 7265 7320 6172 653a 0a0a   features are:..
-000005b0: 2d20 2a2a 4561 7379 2074 6f20 636f 6465  - **Easy to code
-000005c0: 3a2a 2a20 4561 7379 2074 6f20 7573 6520  :** Easy to use 
-000005d0: 616e 6420 6561 7379 2074 6f20 6c65 6172  and easy to lear
-000005e0: 6e0a 0a2d 202a 2a53 7461 6e64 6172 6420  n..- **Standard 
-000005f0: 646f 6375 6d65 6e74 2073 7065 6369 6669  document specifi
-00000600: 6361 7469 6f6e 3a2a 2a20 4261 7365 6420  cation:** Based 
-00000610: 6f6e 205b 4f70 656e 4150 4920 5370 6563  on [OpenAPI Spec
-00000620: 6966 6963 6174 696f 6e5d 2868 7474 7073  ification](https
-00000630: 3a2f 2f73 7065 632e 6f70 656e 6170 6973  ://spec.openapis
-00000640: 2e6f 7267 2f6f 6173 2f76 332e 312e 3029  .org/oas/v3.1.0)
-00000650: 0a0a 2d20 2a2a 496e 7465 7261 6374 6976  ..- **Interactiv
-00000660: 6520 4f70 656e 4150 4920 646f 6375 6d65  e OpenAPI docume
-00000670: 6e74 6174 696f 6e3a 2a2a 205b 5377 6167  ntation:** [Swag
-00000680: 6765 725d 2868 7474 7073 3a2f 2f67 6974  ger](https://git
-00000690: 6875 622e 636f 6d2f 7377 6167 6765 722d  hub.com/swagger-
-000006a0: 6170 692f 7377 6167 6765 722d 7569 292c  api/swagger-ui),
-000006b0: 205b 5265 646f 635d 2868 7474 7073 3a2f   [Redoc](https:/
-000006c0: 2f67 6974 6875 622e 636f 6d2f 5265 646f  /github.com/Redo
-000006d0: 636c 792f 7265 646f 6329 2061 6e64 205b  cly/redoc) and [
-000006e0: 5261 7069 446f 635d 2868 7474 7073 3a2f  RapiDoc](https:/
-000006f0: 2f67 6974 6875 622e 636f 6d2f 7261 7069  /github.com/rapi
-00000700: 2d64 6f63 2f52 6170 6944 6f63 290a 2020  -doc/RapiDoc).  
-00000710: 0a2d 202a 2a44 6174 6120 7661 6c69 6461  .- **Data valida
-00000720: 7469 6f6e 3a2a 2a20 4661 7374 2064 6174  tion:** Fast dat
-00000730: 6120 7665 7269 6669 6361 7469 6f6e 2062  a verification b
-00000740: 6173 6564 206f 6e20 5b50 7964 616e 7469  ased on [Pydanti
-00000750: 635d 2868 7474 7073 3a2f 2f67 6974 6875  c](https://githu
-00000760: 622e 636f 6d2f 7079 6461 6e74 6963 2f70  b.com/pydantic/p
-00000770: 7964 616e 7469 6329 0a0a 2d20 2a2a 4175  ydantic)..- **Au
-00000780: 7468 6f72 697a 6174 696f 6e3a 2a2a 2053  thorization:** S
-00000790: 7570 706f 7274 2074 6f20 7265 6c6f 6164  upport to reload
-000007a0: 2061 7574 686f 7269 7a61 7469 6f6e 7320   authorizations 
-000007b0: 696e 2053 7761 6767 6572 2055 490a 0a23  in Swagger UI..#
-000007c0: 2320 5265 7175 6972 656d 656e 7473 0a0a  # Requirements..
-000007d0: 5079 7468 6f6e 2033 2e38 2b0a 0a66 6c61  Python 3.8+..fla
-000007e0: 736b 2d6f 7065 6e61 7069 3320 6973 2064  sk-openapi3 is d
-000007f0: 6570 656e 6465 6e74 206f 6e20 7468 6520  ependent on the 
-00000800: 666f 6c6c 6f77 696e 6720 6c69 6272 6172  following librar
-00000810: 6965 733a 0a0a 2d20 5b46 6c61 736b 5d28  ies:..- [Flask](
-00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000830: 6f6d 2f70 616c 6c65 7473 2f66 6c61 736b  om/pallets/flask
-00000840: 2920 666f 7220 7468 6520 7765 6220 6170  ) for the web ap
-00000850: 702e 0a2d 205b 5079 6461 6e74 6963 5d28  p..- [Pydantic](
-00000860: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000870: 6f6d 2f70 7964 616e 7469 632f 7079 6461  om/pydantic/pyda
-00000880: 6e74 6963 2920 666f 7220 7468 6520 6461  ntic) for the da
-00000890: 7461 2076 616c 6964 6174 696f 6e2e 0a0a  ta validation...
-000008a0: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-000008b0: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-000008c0: 7461 6c6c 202d 5520 666c 6173 6b2d 6f70  tall -U flask-op
-000008d0: 656e 6170 6933 0a60 6060 0a0a 6f72 0a0a  enapi3.```..or..
-000008e0: 6060 6062 6173 680a 636f 6e64 6120 696e  ```bash.conda in
-000008f0: 7374 616c 6c20 2d63 2063 6f6e 6461 2d66  stall -c conda-f
-00000900: 6f72 6765 2066 6c61 736b 2d6f 7065 6e61  orge flask-opena
-00000910: 7069 330a 6060 600a 0a3c 6465 7461 696c  pi3.```..<detail
-00000920: 7320 6d61 726b 646f 776e 3d22 626c 6f63  s markdown="bloc
-00000930: 6b22 3e0a 3c73 756d 6d61 7279 3e4f 7074  k">.<summary>Opt
-00000940: 696f 6e61 6c20 6465 7065 6e64 656e 6369  ional dependenci
-00000950: 6573 3c2f 7375 6d6d 6172 793e 0a0a 2d20  es</summary>..- 
-00000960: 5b70 7974 686f 6e2d 656d 6169 6c2d 7661  [python-email-va
-00000970: 6c69 6461 746f 725d 2868 7474 7073 3a2f  lidator](https:/
-00000980: 2f67 6974 6875 622e 636f 6d2f 4a6f 7368  /github.com/Josh
-00000990: 4461 7461 2f70 7974 686f 6e2d 656d 6169  Data/python-emai
-000009a0: 6c2d 7661 6c69 6461 746f 7229 2073 7570  l-validator) sup
-000009b0: 706f 7274 7320 656d 6169 6c20 7665 7269  ports email veri
-000009c0: 6669 6361 7469 6f6e 2e0a 2d20 5b70 7974  fication..- [pyt
-000009d0: 686f 6e2d 646f 7465 6e76 5d28 6874 7470  hon-dotenv](http
-000009e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-000009f0: 6865 736b 756d 6172 2f70 7974 686f 6e2d  heskumar/python-
-00000a00: 646f 7465 6e76 2372 6561 646d 6529 2065  dotenv#readme) e
-00000a10: 6e61 626c 6573 2073 7570 706f 7274 2066  nables support f
-00000a20: 6f72 205b 456e 7669 726f 6e6d 656e 7420  or [Environment 
-00000a30: 5661 7269 6162 6c65 7320 4672 6f6d 2064  Variables From d
-00000a40: 6f74 656e 765d 2868 7474 7073 3a2f 2f66  otenv](https://f
-00000a50: 6c61 736b 2e70 616c 6c65 7473 7072 6f6a  lask.palletsproj
-00000a60: 6563 7473 2e63 6f6d 2f65 6e2f 6c61 7465  ects.com/en/late
-00000a70: 7374 2f63 6c69 2f23 646f 7465 6e76 2920  st/cli/#dotenv) 
-00000a80: 7768 656e 2072 756e 6e69 6e67 2060 666c  when running `fl
-00000a90: 6173 6b60 2063 6f6d 6d61 6e64 732e 0a2d  ask` commands..-
-00000aa0: 205b 7079 7961 6d6c 5d28 6874 7470 733a   [pyyaml](https:
-00000ab0: 2f2f 6769 7468 7562 2e63 6f6d 2f79 616d  //github.com/yam
-00000ac0: 6c2f 7079 7961 6d6c 2920 6973 2075 7365  l/pyyaml) is use
-00000ad0: 6420 746f 206f 7574 7075 7420 7468 6520  d to output the 
-00000ae0: 4f70 656e 4150 4920 646f 6375 6d65 6e74  OpenAPI document
-00000af0: 2069 6e20 7961 6d6c 2066 6f72 6d61 742e   in yaml format.
-00000b00: 0a2d 205b 6173 6769 7265 665d 2868 7474  .- [asgiref](htt
-00000b10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b20: 646a 616e 676f 2f61 7367 6972 6566 2920  django/asgiref) 
-00000b30: 616c 6c6f 7773 2076 6965 7773 2074 6f20  allows views to 
-00000b40: 6265 2064 6566 696e 6564 2077 6974 6820  be defined with 
-00000b50: 6061 7379 6e63 2064 6566 6020 616e 6420  `async def` and 
-00000b60: 7573 6520 6061 7761 6974 602e 0a0a 546f  use `await`...To
-00000b70: 2069 6e73 7461 6c6c 2074 6865 7365 2064   install these d
-00000b80: 6570 656e 6465 6e63 6965 7320 7769 7468  ependencies with
-00000b90: 2066 6c61 736b 2d6f 7065 6e61 7069 333a   flask-openapi3:
-00000ba0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
-00000bb0: 7374 616c 6c20 666c 6173 6b2d 6f70 656e  stall flask-open
-00000bc0: 6170 6933 5b79 616d 6c5d 0a23 206f 720a  api3[yaml].# or.
-00000bd0: 7069 7020 696e 7374 616c 6c20 666c 6173  pip install flas
-00000be0: 6b2d 6f70 656e 6170 6933 5b61 7379 6e63  k-openapi3[async
-00000bf0: 5d0a 2320 6f72 0a70 6970 2069 6e73 7461  ].# or.pip insta
-00000c00: 6c6c 2066 6c61 736b 2d6f 7065 6e61 7069  ll flask-openapi
-00000c10: 335b 646f 7465 6e76 5d0a 2320 6f72 0a70  3[dotenv].# or.p
-00000c20: 6970 2069 6e73 7461 6c6c 2066 6c61 736b  ip install flask
-00000c30: 2d6f 7065 6e61 7069 335b 656d 6169 6c5d  -openapi3[email]
-00000c40: 0a23 206f 7220 616c 6c0a 7069 7020 696e  .# or all.pip in
-00000c50: 7374 616c 6c20 666c 6173 6b2d 6f70 656e  stall flask-open
-00000c60: 6170 6933 5b79 616d 6c2c 6173 796e 632c  api3[yaml,async,
-00000c70: 646f 7465 6e76 2c65 6d61 696c 5d0a 2320  dotenv,email].# 
-00000c80: 6f72 206d 616e 7561 6c6c 790a 7069 7020  or manually.pip 
-00000c90: 696e 7374 616c 6c20 7079 7961 6d6c 2061  install pyyaml a
-00000ca0: 7367 6972 6566 2070 7974 686f 6e2d 646f  sgiref python-do
-00000cb0: 7465 6e76 2065 6d61 696c 2d76 616c 6964  tenv email-valid
-00000cc0: 6174 6f72 0a60 6060 0a3c 2f64 6574 6169  ator.```.</detai
-00000cd0: 6c73 3e0a 0a23 2320 4120 5369 6d70 6c65  ls>..## A Simple
-00000ce0: 2045 7861 6d70 6c65 0a0a 4865 7265 2773   Example..Here's
-00000cf0: 2061 2073 696d 706c 6520 6578 616d 706c   a simple exampl
-00000d00: 652c 2066 7572 7468 6572 2067 6f20 746f  e, further go to
-00000d10: 2074 6865 205b 4578 616d 706c 655d 2868   the [Example](h
-00000d20: 7474 7073 3a2f 2f6c 756f 6c69 6e67 6368  ttps://luolingch
-00000d30: 756e 2e67 6974 6875 622e 696f 2f66 6c61  un.github.io/fla
-00000d40: 736b 2d6f 7065 6e61 7069 332f 6c61 7465  sk-openapi3/late
-00000d50: 7374 2f45 7861 6d70 6c65 2f29 2e0a 0a60  st/Example/)...`
-00000d60: 6060 7079 7468 6f6e 0a66 726f 6d20 7079  ``python.from py
-00000d70: 6461 6e74 6963 2069 6d70 6f72 7420 4261  dantic import Ba
-00000d80: 7365 4d6f 6465 6c0a 0a66 726f 6d20 666c  seModel..from fl
-00000d90: 6173 6b5f 6f70 656e 6170 6933 2069 6d70  ask_openapi3 imp
-00000da0: 6f72 7420 496e 666f 2c20 5461 670a 6672  ort Info, Tag.fr
-00000db0: 6f6d 2066 6c61 736b 5f6f 7065 6e61 7069  om flask_openapi
-00000dc0: 3320 696d 706f 7274 204f 7065 6e41 5049  3 import OpenAPI
-00000dd0: 0a0a 696e 666f 203d 2049 6e66 6f28 7469  ..info = Info(ti
-00000de0: 746c 653d 2262 6f6f 6b20 4150 4922 2c20  tle="book API", 
-00000df0: 7665 7273 696f 6e3d 2231 2e30 2e30 2229  version="1.0.0")
-00000e00: 0a61 7070 203d 204f 7065 6e41 5049 285f  .app = OpenAPI(_
-00000e10: 5f6e 616d 655f 5f2c 2069 6e66 6f3d 696e  _name__, info=in
-00000e20: 666f 290a 0a62 6f6f 6b5f 7461 6720 3d20  fo)..book_tag = 
-00000e30: 5461 6728 6e61 6d65 3d22 626f 6f6b 222c  Tag(name="book",
-00000e40: 2064 6573 6372 6970 7469 6f6e 3d22 536f   description="So
-00000e50: 6d65 2042 6f6f 6b22 290a 0a0a 636c 6173  me Book")...clas
-00000e60: 7320 426f 6f6b 5175 6572 7928 4261 7365  s BookQuery(Base
-00000e70: 4d6f 6465 6c29 3a0a 2020 2020 6167 653a  Model):.    age:
-00000e80: 2069 6e74 0a20 2020 2061 7574 686f 723a   int.    author:
-00000e90: 2073 7472 0a0a 0a40 6170 702e 6765 7428   str...@app.get(
-00000ea0: 222f 626f 6f6b 222c 2073 756d 6d61 7279  "/book", summary
-00000eb0: 3d22 6765 7420 626f 6f6b 7322 2c20 7461  ="get books", ta
-00000ec0: 6773 3d5b 626f 6f6b 5f74 6167 5d29 0a64  gs=[book_tag]).d
-00000ed0: 6566 2067 6574 5f62 6f6f 6b28 7175 6572  ef get_book(quer
-00000ee0: 793a 2042 6f6f 6b51 7565 7279 293a 0a20  y: BookQuery):. 
-00000ef0: 2020 2022 2222 0a20 2020 2074 6f20 6765     """.    to ge
-00000f00: 7420 616c 6c20 626f 6f6b 730a 2020 2020  t all books.    
-00000f10: 2222 220a 2020 2020 7265 7475 726e 207b  """.    return {
-00000f20: 0a20 2020 2020 2020 2022 636f 6465 223a  .        "code":
-00000f30: 2030 2c0a 2020 2020 2020 2020 226d 6573   0,.        "mes
-00000f40: 7361 6765 223a 2022 6f6b 222c 0a20 2020  sage": "ok",.   
-00000f50: 2020 2020 2022 6461 7461 223a 205b 0a20       "data": [. 
-00000f60: 2020 2020 2020 2020 2020 207b 2262 6964             {"bid
-00000f70: 223a 2031 2c20 2261 6765 223a 2071 7565  ": 1, "age": que
-00000f80: 7279 2e61 6765 2c20 2261 7574 686f 7222  ry.age, "author"
-00000f90: 3a20 7175 6572 792e 6175 7468 6f72 7d2c  : query.author},
-00000fa0: 0a20 2020 2020 2020 2020 2020 207b 2262  .            {"b
-00000fb0: 6964 223a 2032 2c20 2261 6765 223a 2071  id": 2, "age": q
-00000fc0: 7565 7279 2e61 6765 2c20 2261 7574 686f  uery.age, "autho
-00000fd0: 7222 3a20 7175 6572 792e 6175 7468 6f72  r": query.author
-00000fe0: 7d0a 2020 2020 2020 2020 5d0a 2020 2020  }.        ].    
-00000ff0: 7d0a 0a0a 6966 205f 5f6e 616d 655f 5f20  }...if __name__ 
-00001000: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a20  == "__main__":. 
-00001010: 2020 2061 7070 2e72 756e 2864 6562 7567     app.run(debug
-00001020: 3d54 7275 6529 0a60 6060 0a0a 3c64 6574  =True).```..<det
-00001030: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e43  ails>.<summary>C
-00001040: 6c61 7373 2d62 6173 6564 2041 5049 2056  lass-based API V
-00001050: 6965 7720 4578 616d 706c 653c 2f73 756d  iew Example</sum
-00001060: 6d61 7279 3e0a 0a60 6060 7079 7468 6f6e  mary>..```python
-00001070: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
-00001080: 6f72 7420 4f70 7469 6f6e 616c 0a0a 6672  ort Optional..fr
-00001090: 6f6d 2070 7964 616e 7469 6320 696d 706f  om pydantic impo
-000010a0: 7274 2042 6173 654d 6f64 656c 2c20 4669  rt BaseModel, Fi
-000010b0: 656c 640a 0a66 726f 6d20 666c 6173 6b5f  eld..from flask_
-000010c0: 6f70 656e 6170 6933 2069 6d70 6f72 7420  openapi3 import 
-000010d0: 4f70 656e 4150 492c 2054 6167 2c20 496e  OpenAPI, Tag, In
-000010e0: 666f 2c20 4150 4956 6965 770a 0a0a 696e  fo, APIView...in
-000010f0: 666f 203d 2049 6e66 6f28 7469 746c 653d  fo = Info(title=
-00001100: 2762 6f6f 6b20 4150 4927 2c20 7665 7273  'book API', vers
-00001110: 696f 6e3d 2731 2e30 2e30 2729 0a61 7070  ion='1.0.0').app
-00001120: 203d 204f 7065 6e41 5049 285f 5f6e 616d   = OpenAPI(__nam
-00001130: 655f 5f2c 2069 6e66 6f3d 696e 666f 290a  e__, info=info).
-00001140: 0a61 7069 5f76 6965 7720 3d20 4150 4956  .api_view = APIV
-00001150: 6965 7728 7572 6c5f 7072 6566 6978 3d22  iew(url_prefix="
-00001160: 2f61 7069 2f76 3122 2c20 7669 6577 5f74  /api/v1", view_t
-00001170: 6167 733d 5b54 6167 286e 616d 653d 2262  ags=[Tag(name="b
-00001180: 6f6f 6b22 295d 290a 0a0a 636c 6173 7320  ook")])...class 
-00001190: 426f 6f6b 5061 7468 2842 6173 654d 6f64  BookPath(BaseMod
-000011a0: 656c 293a 0a20 2020 2069 643a 2069 6e74  el):.    id: int
-000011b0: 203d 2046 6965 6c64 282e 2e2e 2c20 6465   = Field(..., de
-000011c0: 7363 7269 7074 696f 6e3d 2262 6f6f 6b20  scription="book 
-000011d0: 4944 2229 0a0a 0a63 6c61 7373 2042 6f6f  ID")...class Boo
-000011e0: 6b51 7565 7279 2842 6173 654d 6f64 656c  kQuery(BaseModel
-000011f0: 293a 0a20 2020 2061 6765 3a20 4f70 7469  ):.    age: Opti
-00001200: 6f6e 616c 5b69 6e74 5d20 3d20 4669 656c  onal[int] = Fiel
-00001210: 6428 4e6f 6e65 2c20 6465 7363 7269 7074  d(None, descript
-00001220: 696f 6e3d 2741 6765 2729 0a0a 0a63 6c61  ion='Age')...cla
-00001230: 7373 2042 6f6f 6b42 6f64 7928 4261 7365  ss BookBody(Base
-00001240: 4d6f 6465 6c29 3a0a 2020 2020 6167 653a  Model):.    age:
-00001250: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-00001260: 2046 6965 6c64 282e 2e2e 2c20 6765 3d32   Field(..., ge=2
-00001270: 2c20 6c65 3d34 2c20 6465 7363 7269 7074  , le=4, descript
-00001280: 696f 6e3d 2741 6765 2729 0a20 2020 2061  ion='Age').    a
-00001290: 7574 686f 723a 2073 7472 203d 2046 6965  uthor: str = Fie
-000012a0: 6c64 284e 6f6e 652c 206d 696e 5f6c 656e  ld(None, min_len
-000012b0: 6774 683d 322c 206d 6178 5f6c 656e 6774  gth=2, max_lengt
-000012c0: 683d 342c 2064 6573 6372 6970 7469 6f6e  h=4, description
-000012d0: 3d27 4175 7468 6f72 2729 0a0a 0a40 6170  ='Author')...@ap
-000012e0: 695f 7669 6577 2e72 6f75 7465 2822 2f62  i_view.route("/b
-000012f0: 6f6f 6b22 290a 636c 6173 7320 426f 6f6b  ook").class Book
-00001300: 4c69 7374 4150 4956 6965 773a 0a20 2020  ListAPIView:.   
-00001310: 2061 203d 2031 0a0a 2020 2020 4061 7069   a = 1..    @api
-00001320: 5f76 6965 772e 646f 6328 7375 6d6d 6172  _view.doc(summar
-00001330: 793d 2267 6574 2062 6f6f 6b20 6c69 7374  y="get book list
-00001340: 2229 0a20 2020 2064 6566 2067 6574 2873  ").    def get(s
-00001350: 656c 662c 2071 7565 7279 3a20 426f 6f6b  elf, query: Book
-00001360: 5175 6572 7929 3a0a 2020 2020 2020 2020  Query):.        
-00001370: 7072 696e 7428 7365 6c66 2e61 290a 2020  print(self.a).  
-00001380: 2020 2020 2020 7265 7475 726e 2071 7565        return que
-00001390: 7279 2e6d 6f64 656c 5f64 756d 705f 6a73  ry.model_dump_js
-000013a0: 6f6e 2829 0a0a 2020 2020 4061 7069 5f76  on()..    @api_v
-000013b0: 6965 772e 646f 6328 7375 6d6d 6172 793d  iew.doc(summary=
-000013c0: 2263 7265 6174 6520 626f 6f6b 2229 0a20  "create book"). 
-000013d0: 2020 2064 6566 2070 6f73 7428 7365 6c66     def post(self
-000013e0: 2c20 626f 6479 3a20 426f 6f6b 426f 6479  , body: BookBody
-000013f0: 293a 0a20 2020 2020 2020 2022 2222 6465  ):.        """de
-00001400: 7363 7269 7074 696f 6e20 666f 7220 6120  scription for a 
-00001410: 6372 6561 7465 6420 626f 6f6b 2222 220a  created book""".
-00001420: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-00001430: 6f64 792e 6d6f 6465 6c5f 6475 6d70 5f6a  ody.model_dump_j
-00001440: 736f 6e28 290a 0a0a 4061 7069 5f76 6965  son()...@api_vie
-00001450: 772e 726f 7574 6528 222f 626f 6f6b 2f3c  w.route("/book/<
-00001460: 6964 3e22 290a 636c 6173 7320 426f 6f6b  id>").class Book
-00001470: 4150 4956 6965 773a 0a20 2020 2040 6170  APIView:.    @ap
-00001480: 695f 7669 6577 2e64 6f63 2873 756d 6d61  i_view.doc(summa
-00001490: 7279 3d22 6765 7420 626f 6f6b 2229 0a20  ry="get book"). 
-000014a0: 2020 2064 6566 2067 6574 2873 656c 662c     def get(self,
-000014b0: 2070 6174 683a 2042 6f6f 6b50 6174 6829   path: BookPath)
-000014c0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-000014d0: 7061 7468 290a 2020 2020 2020 2020 7265  path).        re
-000014e0: 7475 726e 2022 6765 7422 0a0a 2020 2020  turn "get"..    
-000014f0: 4061 7069 5f76 6965 772e 646f 6328 7375  @api_view.doc(su
-00001500: 6d6d 6172 793d 2275 7064 6174 6520 626f  mmary="update bo
-00001510: 6f6b 2229 0a20 2020 2064 6566 2070 7574  ok").    def put
-00001520: 2873 656c 662c 2070 6174 683a 2042 6f6f  (self, path: Boo
-00001530: 6b50 6174 6829 3a0a 2020 2020 2020 2020  kPath):.        
-00001540: 7072 696e 7428 7061 7468 290a 2020 2020  print(path).    
-00001550: 2020 2020 7265 7475 726e 2022 7075 7422      return "put"
-00001560: 0a0a 2020 2020 4061 7069 5f76 6965 772e  ..    @api_view.
-00001570: 646f 6328 7375 6d6d 6172 793d 2264 656c  doc(summary="del
-00001580: 6574 6520 626f 6f6b 222c 2064 6570 7265  ete book", depre
-00001590: 6361 7465 643d 5472 7565 290a 2020 2020  cated=True).    
-000015a0: 6465 6620 6465 6c65 7465 2873 656c 662c  def delete(self,
-000015b0: 2070 6174 683a 2042 6f6f 6b50 6174 6829   path: BookPath)
-000015c0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-000015d0: 7061 7468 290a 2020 2020 2020 2020 7265  path).        re
-000015e0: 7475 726e 2022 6465 6c65 7465 220a 0a0a  turn "delete"...
-000015f0: 6170 702e 7265 6769 7374 6572 5f61 7069  app.register_api
-00001600: 5f76 6965 7728 6170 695f 7669 6577 290a  _view(api_view).
-00001610: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00001620: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00001630: 6170 702e 7275 6e28 6465 6275 673d 5472  app.run(debug=Tr
-00001640: 7565 290a 6060 600a 3c2f 6465 7461 696c  ue).```.</detail
-00001650: 733e 0a0a 2323 2041 5049 2044 6f63 756d  s>..## API Docum
-00001660: 656e 740a 0a52 756e 2074 6865 205b 7369  ent..Run the [si
-00001670: 6d70 6c65 2065 7861 6d70 6c65 5d28 6874  mple example](ht
-00001680: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001690: 2f6c 756f 6c69 6e67 6368 756e 2f66 6c61  /luolingchun/fla
-000016a0: 736b 2d6f 7065 6e61 7069 332f 626c 6f62  sk-openapi3/blob
-000016b0: 2f6d 6173 7465 722f 6578 616d 706c 6573  /master/examples
-000016c0: 2f73 696d 706c 655f 6465 6d6f 2e70 7929  /simple_demo.py)
-000016d0: 2c20 616e 6420 676f 2074 6f20 6874 7470  , and go to http
-000016e0: 3a2f 2f31 3237 2e30 2e30 2e31 3a35 3030  ://127.0.0.1:500
-000016f0: 302f 6f70 656e 6170 692e 0a0a 596f 7520  0/openapi...You 
-00001700: 7769 6c6c 2073 6565 2074 6865 2064 6f63  will see the doc
-00001710: 756d 656e 7461 7469 6f6e 3a20 5b53 7761  umentation: [Swa
-00001720: 6767 6572 5d28 6874 7470 733a 2f2f 6769  gger](https://gi
-00001730: 7468 7562 2e63 6f6d 2f73 7761 6767 6572  thub.com/swagger
-00001740: 2d61 7069 2f73 7761 6767 6572 2d75 6929  -api/swagger-ui)
-00001750: 2c20 5b52 6564 6f63 5d28 6874 7470 733a  , [Redoc](https:
-00001760: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6564  //github.com/Red
-00001770: 6f63 6c79 2f72 6564 6f63 2920 616e 6420  ocly/redoc) and 
-00001780: 5b52 6170 6944 6f63 5d28 6874 7470 733a  [RapiDoc](https:
-00001790: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6170  //github.com/rap
-000017a0: 692d 646f 632f 5261 7069 446f 6329 2e0a  i-doc/RapiDoc)..
-000017b0: 0a21 5b6f 7065 6e61 7069 5d28 6874 7470  .![openapi](http
-000017c0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000017d0: 6572 636f 6e74 656e 742e 636f 6d2f 6c75  ercontent.com/lu
-000017e0: 6f6c 696e 6763 6875 6e2f 666c 6173 6b2d  olingchun/flask-
-000017f0: 6f70 656e 6170 6933 2f6d 6173 7465 722f  openapi3/master/
-00001800: 646f 6373 2f69 6d61 6765 732f 6f70 656e  docs/images/open
-00001810: 6170 692e 706e 6729 0a21 5b6f 7065 6e61  api.png).![opena
-00001820: 7069 2d73 7761 6767 6572 5d28 6874 7470  pi-swagger](http
-00001830: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00001840: 6572 636f 6e74 656e 742e 636f 6d2f 6c75  ercontent.com/lu
-00001850: 6f6c 696e 6763 6875 6e2f 666c 6173 6b2d  olingchun/flask-
-00001860: 6f70 656e 6170 6933 2f6d 6173 7465 722f  openapi3/master/
-00001870: 646f 6373 2f69 6d61 6765 732f 6f70 656e  docs/images/open
-00001880: 6170 692d 7377 6167 6765 722e 706e 6729  api-swagger.png)
-00001890: 0a21 5b6f 7065 6e61 7069 2d72 6564 6f63  .![openapi-redoc
-000018a0: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
-000018b0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000018c0: 636f 6d2f 6c75 6f6c 696e 6763 6875 6e2f  com/luolingchun/
-000018d0: 666c 6173 6b2d 6f70 656e 6170 6933 2f6d  flask-openapi3/m
-000018e0: 6173 7465 722f 646f 6373 2f69 6d61 6765  aster/docs/image
-000018f0: 732f 6f70 656e 6170 692d 7265 646f 632e  s/openapi-redoc.
-00001900: 706e 6729 0a21 5b6f 7065 6e61 7069 2d52  png).![openapi-R
-00001910: 6170 6944 6f63 5d28 6874 7470 733a 2f2f  apiDoc](https://
-00001920: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00001930: 6e74 656e 742e 636f 6d2f 6c75 6f6c 696e  ntent.com/luolin
-00001940: 6763 6875 6e2f 666c 6173 6b2d 6f70 656e  gchun/flask-open
-00001950: 6170 6933 2f6d 6173 7465 722f 646f 6373  api3/master/docs
-00001960: 2f69 6d61 6765 732f 6f70 656e 6170 692d  /images/openapi-
-00001970: 7261 7069 646f 632e 706e 6729 0a         rapidoc.png).
+00000010: 6572 223e 0d0a 2020 2020 3c61 2068 7265  er">..    <a hre
+00000020: 663d 2268 7474 7073 3a2f 2f6c 756f 6c69  f="https://luoli
+00000030: 6e67 6368 756e 2e67 6974 6875 622e 696f  ngchun.github.io
+00000040: 2f66 6c61 736b 2d6f 7065 6e61 7069 332f  /flask-openapi3/
+00000050: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000060: 223e 0d0a 2020 2020 2020 2020 3c69 6d67  ">..        <img
+00000070: 2063 6c61 7373 3d22 6f66 662d 676c 6222   class="off-glb"
+00000080: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000090: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000000a0: 656e 742e 636f 6d2f 6c75 6f6c 696e 6763  ent.com/luolingc
+000000b0: 6875 6e2f 666c 6173 6b2d 6f70 656e 6170  hun/flask-openap
+000000c0: 6933 2f6d 6173 7465 722f 646f 6373 2f69  i3/master/docs/i
+000000d0: 6d61 6765 732f 6c6f 676f 2d74 6578 742e  mages/logo-text.
+000000e0: 7376 6722 200d 0a20 2020 2020 2020 2020  svg" ..         
+000000f0: 2020 2020 7769 6474 683d 2236 3025 2220      width="60%" 
+00000100: 6865 6967 6874 3d22 6175 746f 2220 616c  height="auto" al
+00000110: 743d 226c 6f67 6f22 3e0d 0a20 2020 203c  t="logo">..    <
+00000120: 2f61 3e0d 0a3c 2f64 6976 3e0d 0a3c 7020  /a>..</div>..<p 
+00000130: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000140: 0a20 2020 203c 656d 3e47 656e 6572 6174  .    <em>Generat
+00000150: 6520 5245 5354 2041 5049 2061 6e64 204f  e REST API and O
+00000160: 7065 6e41 5049 2064 6f63 756d 656e 7461  penAPI documenta
+00000170: 7469 6f6e 2066 6f72 2079 6f75 7220 466c  tion for your Fl
+00000180: 6173 6b20 7072 6f6a 6563 742e 3c2f 656d  ask project.</em
+00000190: 3e0d 0a3c 2f70 3e0d 0a3c 7020 616c 6967  >..</p>..<p alig
+000001a0: 6e3d 2263 656e 7465 7222 3e0d 0a20 2020  n="center">..   
+000001b0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 756f  //github.com/luo
+000001d0: 6c69 6e67 6368 756e 2f66 6c61 736b 2d6f  lingchun/flask-o
+000001e0: 7065 6e61 7069 332f 6163 7469 6f6e 732f  penapi3/actions/
+000001f0: 776f 726b 666c 6f77 732f 7465 7374 732e  workflows/tests.
+00000200: 796d 6c22 2074 6172 6765 743d 225f 626c  yml" target="_bl
+00000210: 616e 6b22 3e0d 0a20 2020 2020 2020 203c  ank">..        <
+00000220: 696d 6720 636c 6173 733d 226f 6666 2d67  img class="off-g
+00000230: 6c62 2220 7372 633d 2268 7474 7073 3a2f  lb" src="https:/
+00000240: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000250: 6769 7468 7562 2f61 6374 696f 6e73 2f77  github/actions/w
+00000260: 6f72 6b66 6c6f 772f 7374 6174 7573 2f6c  orkflow/status/l
+00000270: 756f 6c69 6e67 6368 756e 2f66 6c61 736b  uolingchun/flask
+00000280: 2d6f 7065 6e61 7069 332f 7465 7374 732e  -openapi3/tests.
+00000290: 796d 6c3f 6272 616e 6368 3d6d 6173 7465  yml?branch=maste
+000002a0: 7222 2061 6c74 3d22 7465 7374 223e 0d0a  r" alt="test">..
+000002b0: 2020 2020 3c2f 613e 0d0a 2020 2020 3c61      </a>..    <a
+000002c0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+000002d0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000002e0: 666c 6173 6b2d 6f70 656e 6170 6933 2f22  flask-openapi3/"
+000002f0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000300: 3e0d 0a20 2020 2020 2020 203c 696d 6720  >..        <img 
+00000310: 636c 6173 733d 226f 6666 2d67 6c62 2220  class="off-glb" 
+00000320: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000330: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000340: 2f76 2f66 6c61 736b 2d6f 7065 6e61 7069  /v/flask-openapi
+00000350: 3322 2061 6c74 3d22 7079 7069 223e 0d0a  3" alt="pypi">..
+00000360: 2020 2020 3c2f 613e 0d0a 2020 2020 3c61      </a>..    <a
+00000370: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00000380: 7970 6973 7461 7473 2e6f 7267 2f70 6163  ypistats.org/pac
+00000390: 6b61 6765 732f 666c 6173 6b2d 6f70 656e  kages/flask-open
+000003a0: 6170 6933 2220 7461 7267 6574 3d22 5f62  api3" target="_b
+000003b0: 6c61 6e6b 223e 0d0a 2020 2020 2020 2020  lank">..        
+000003c0: 3c69 6d67 2063 6c61 7373 3d22 6f66 662d  <img class="off-
+000003d0: 676c 6222 2073 7263 3d22 6874 7470 733a  glb" src="https:
+000003e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000003f0: 2f70 7970 692f 646d 2f66 6c61 736b 2d6f  /pypi/dm/flask-o
+00000400: 7065 6e61 7069 3322 2061 6c74 3d22 7079  penapi3" alt="py
+00000410: 7069 7374 6174 7322 3e0d 0a20 2020 203c  pistats">..    <
+00000420: 2f61 3e0d 0a20 2020 203c 6120 6872 6566  /a>..    <a href
+00000430: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000440: 7267 2f70 726f 6a65 6374 2f66 6c61 736b  rg/project/flask
+00000450: 2d6f 7065 6e61 7069 332f 2220 7461 7267  -openapi3/" targ
+00000460: 6574 3d22 5f62 6c61 6e6b 223e 0d0a 2020  et="_blank">..  
+00000470: 2020 2020 2020 3c69 6d67 2063 6c61 7373        <img class
+00000480: 3d22 6f66 662d 676c 6222 2073 7263 3d22  ="off-glb" src="
+00000490: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004a0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+000004b0: 7273 696f 6e73 2f66 6c61 736b 2d6f 7065  rsions/flask-ope
+000004c0: 6e61 7069 3322 2061 6c74 3d22 7079 7069  napi3" alt="pypi
+000004d0: 2076 6572 7369 6f6e 7322 3e0d 0a20 2020   versions">..   
+000004e0: 203c 2f61 3e0d 0a3c 2f70 3e0d 0a0d 0a3e   </a>..</p>....>
+000004f0: 2054 6869 7320 6272 616e 6368 2069 7320   This branch is 
+00000500: 696e 2064 6576 656c 6f70 6d65 6e74 2070  in development p
+00000510: 7265 7669 6577 2073 7461 7465 2e0d 0a0d  review state....
+00000520: 0a2a 2a46 6c61 736b 204f 7065 6e41 5049  .**Flask OpenAPI
+00000530: 332a 2a20 6973 2061 2077 6562 2041 5049  3** is a web API
+00000540: 2066 7261 6d65 776f 726b 2062 6173 6564   framework based
+00000550: 206f 6e20 2a2a 466c 6173 6b2a 2a2e 2049   on **Flask**. I
+00000560: 7420 7573 6573 202a 2a50 7964 616e 7469  t uses **Pydanti
+00000570: 632a 2a20 746f 2076 6572 6966 7920 6461  c** to verify da
+00000580: 7461 2061 6e64 2061 7574 6f6d 6174 6963  ta and automatic
+00000590: 0d0a 6765 6e65 7261 7469 6f6e 206f 6620  ..generation of 
+000005a0: 696e 7465 7261 6374 696f 6e20 646f 6375  interaction docu
+000005b0: 6d65 6e74 6174 696f 6e3a 202a 2a53 7761  mentation: **Swa
+000005c0: 6767 6572 2a2a 2c20 2a2a 5265 446f 632a  gger**, **ReDoc*
+000005d0: 2a2c 202a 2a52 6170 6944 6f63 2a2a 2c20  *, **RapiDoc**, 
+000005e0: 6574 632e 0d0a 0d0a 5468 6520 6b65 7920  etc.....The key 
+000005f0: 6665 6174 7572 6573 2061 7265 3a0d 0a0d  features are:...
+00000600: 0a2d 202a 2a45 6173 7920 746f 2063 6f64  .- **Easy to cod
+00000610: 653a 2a2a 2045 6173 7920 746f 2075 7365  e:** Easy to use
+00000620: 2061 6e64 2065 6173 7920 746f 206c 6561   and easy to lea
+00000630: 726e 0d0a 0d0a 2d20 2a2a 5374 616e 6461  rn....- **Standa
+00000640: 7264 2064 6f63 756d 656e 7420 7370 6563  rd document spec
+00000650: 6966 6963 6174 696f 6e3a 2a2a 2042 6173  ification:** Bas
+00000660: 6564 206f 6e20 5b4f 7065 6e41 5049 2053  ed on [OpenAPI S
+00000670: 7065 6369 6669 6361 7469 6f6e 5d28 6874  pecification](ht
+00000680: 7470 733a 2f2f 7370 6563 2e6f 7065 6e61  tps://spec.opena
+00000690: 7069 732e 6f72 672f 6f61 732f 7633 2e31  pis.org/oas/v3.1
+000006a0: 2e30 290d 0a0d 0a2d 202a 2a49 6e74 6572  .0)....- **Inter
+000006b0: 6163 7469 7665 204f 7065 6e41 5049 2064  active OpenAPI d
+000006c0: 6f63 756d 656e 7461 7469 6f6e 3a2a 2a20  ocumentation:** 
+000006d0: 5b53 7761 6767 6572 5d28 6874 7470 733a  [Swagger](https:
+000006e0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7761  //github.com/swa
+000006f0: 6767 6572 2d61 7069 2f73 7761 6767 6572  gger-api/swagger
+00000700: 2d75 6929 2c20 5b52 6564 6f63 5d28 6874  -ui), [Redoc](ht
+00000710: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000720: 2f52 6564 6f63 6c79 2f72 6564 6f63 292c  /Redocly/redoc),
+00000730: 205b 5261 7069 446f 635d 2868 7474 7073   [RapiDoc](https
+00000740: 3a2f 2f67 6974 6875 622e 636f 6d2f 7261  ://github.com/ra
+00000750: 7069 2d64 6f63 2f52 6170 6944 6f63 292c  pi-doc/RapiDoc),
+00000760: 2065 7463 2e0d 0a20 200d 0a2d 202a 2a44   etc...  ..- **D
+00000770: 6174 6120 7661 6c69 6461 7469 6f6e 3a2a  ata validation:*
+00000780: 2a20 4661 7374 2064 6174 6120 7665 7269  * Fast data veri
+00000790: 6669 6361 7469 6f6e 2062 6173 6564 206f  fication based o
+000007a0: 6e20 5b50 7964 616e 7469 635d 2868 7474  n [Pydantic](htt
+000007b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007c0: 7079 6461 6e74 6963 2f70 7964 616e 7469  pydantic/pydanti
+000007d0: 6329 0d0a 0d0a 2d20 2a2a 4175 7468 6f72  c)....- **Author
+000007e0: 697a 6174 696f 6e3a 2a2a 2053 7570 706f  ization:** Suppo
+000007f0: 7274 2074 6f20 7265 6c6f 6164 2061 7574  rt to reload aut
+00000800: 686f 7269 7a61 7469 6f6e 7320 696e 2053  horizations in S
+00000810: 7761 6767 6572 2055 490d 0a0d 0a23 2320  wagger UI....## 
+00000820: 5265 7175 6972 656d 656e 7473 0d0a 0d0a  Requirements....
+00000830: 5079 7468 6f6e 2033 2e38 2b0d 0a0d 0a66  Python 3.8+....f
+00000840: 6c61 736b 2d6f 7065 6e61 7069 3320 6973  lask-openapi3 is
+00000850: 2064 6570 656e 6465 6e74 206f 6e20 7468   dependent on th
+00000860: 6520 666f 6c6c 6f77 696e 6720 6c69 6272  e following libr
+00000870: 6172 6965 733a 0d0a 0d0a 2d20 5b46 6c61  aries:....- [Fla
+00000880: 736b 5d28 6874 7470 733a 2f2f 6769 7468  sk](https://gith
+00000890: 7562 2e63 6f6d 2f70 616c 6c65 7473 2f66  ub.com/pallets/f
+000008a0: 6c61 736b 2920 666f 7220 7468 6520 7765  lask) for the we
+000008b0: 6220 6170 702e 0d0a 2d20 5b50 7964 616e  b app...- [Pydan
+000008c0: 7469 635d 2868 7474 7073 3a2f 2f67 6974  tic](https://git
+000008d0: 6875 622e 636f 6d2f 7079 6461 6e74 6963  hub.com/pydantic
+000008e0: 2f70 7964 616e 7469 6329 2066 6f72 2074  /pydantic) for t
+000008f0: 6865 2064 6174 6120 7661 6c69 6461 7469  he data validati
+00000900: 6f6e 2e0d 0a0d 0a23 2320 496e 7374 616c  on.....## Instal
+00000910: 6c61 7469 6f6e 0d0a 0d0a 6060 6062 6173  lation....```bas
+00000920: 680d 0a70 6970 2069 6e73 7461 6c6c 202d  h..pip install -
+00000930: 5520 666c 6173 6b2d 6f70 656e 6170 6933  U flask-openapi3
+00000940: 5b73 7761 6767 6572 5d0d 0a60 6060 0d0a  [swagger]..```..
+00000950: 0d0a 6f72 0d0a 0d0a 6060 6062 6173 680d  ..or....```bash.
+00000960: 0a63 6f6e 6461 2069 6e73 7461 6c6c 202d  .conda install -
+00000970: 6320 636f 6e64 612d 666f 7267 6520 666c  c conda-forge fl
+00000980: 6173 6b2d 6f70 656e 6170 6933 5b73 7761  ask-openapi3[swa
+00000990: 6767 6572 5d0d 0a60 6060 0d0a 0d0a 3c64  gger]..```....<d
+000009a0: 6574 6169 6c73 206d 6172 6b64 6f77 6e3d  etails markdown=
+000009b0: 2262 6c6f 636b 223e 0d0a 3c73 756d 6d61  "block">..<summa
+000009c0: 7279 3e4f 7074 696f 6e61 6c20 6465 7065  ry>Optional depe
+000009d0: 6e64 656e 6369 6573 3c2f 7375 6d6d 6172  ndencies</summar
+000009e0: 793e 0d0a 0d0a 2d20 5b70 7974 686f 6e2d  y>....- [python-
+000009f0: 656d 6169 6c2d 7661 6c69 6461 746f 725d  email-validator]
+00000a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000a10: 636f 6d2f 4a6f 7368 4461 7461 2f70 7974  com/JoshData/pyt
+00000a20: 686f 6e2d 656d 6169 6c2d 7661 6c69 6461  hon-email-valida
+00000a30: 746f 7229 2073 7570 706f 7274 7320 656d  tor) supports em
+00000a40: 6169 6c20 7665 7269 6669 6361 7469 6f6e  ail verification
+00000a50: 2e0d 0a2d 205b 7079 7468 6f6e 2d64 6f74  ...- [python-dot
+00000a60: 656e 765d 2868 7474 7073 3a2f 2f67 6974  env](https://git
+00000a70: 6875 622e 636f 6d2f 7468 6573 6b75 6d61  hub.com/theskuma
+00000a80: 722f 7079 7468 6f6e 2d64 6f74 656e 7623  r/python-dotenv#
+00000a90: 7265 6164 6d65 2920 656e 6162 6c65 7320  readme) enables 
+00000aa0: 7375 7070 6f72 7420 666f 7220 5b45 6e76  support for [Env
+00000ab0: 6972 6f6e 6d65 6e74 2056 6172 6961 626c  ironment Variabl
+00000ac0: 6573 2046 726f 6d20 646f 7465 6e76 5d28  es From dotenv](
+00000ad0: 6874 7470 733a 2f2f 666c 6173 6b2e 7061  https://flask.pa
+00000ae0: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
+00000af0: 6d2f 656e 2f6c 6174 6573 742f 636c 692f  m/en/latest/cli/
+00000b00: 2364 6f74 656e 7629 2077 6865 6e20 7275  #dotenv) when ru
+00000b10: 6e6e 696e 6720 6066 6c61 736b 6020 636f  nning `flask` co
+00000b20: 6d6d 616e 6473 2e0d 0a2d 205b 7079 7961  mmands...- [pyya
+00000b30: 6d6c 5d28 6874 7470 733a 2f2f 6769 7468  ml](https://gith
+00000b40: 7562 2e63 6f6d 2f79 616d 6c2f 7079 7961  ub.com/yaml/pyya
+00000b50: 6d6c 2920 6973 2075 7365 6420 746f 206f  ml) is used to o
+00000b60: 7574 7075 7420 7468 6520 4f70 656e 4150  utput the OpenAP
+00000b70: 4920 646f 6375 6d65 6e74 2069 6e20 7961  I document in ya
+00000b80: 6d6c 2066 6f72 6d61 742e 0d0a 2d20 5b61  ml format...- [a
+00000b90: 7367 6972 6566 5d28 6874 7470 733a 2f2f  sgiref](https://
+00000ba0: 6769 7468 7562 2e63 6f6d 2f64 6a61 6e67  github.com/djang
+00000bb0: 6f2f 6173 6769 7265 6629 2061 6c6c 6f77  o/asgiref) allow
+00000bc0: 7320 7669 6577 7320 746f 2062 6520 6465  s views to be de
+00000bd0: 6669 6e65 6420 7769 7468 2060 6173 796e  fined with `asyn
+00000be0: 6320 6465 6660 2061 6e64 2075 7365 2060  c def` and use `
+00000bf0: 6177 6169 7460 2e0d 0a0d 0a54 6f20 696e  await`.....To in
+00000c00: 7374 616c 6c20 7468 6573 6520 6465 7065  stall these depe
+00000c10: 6e64 656e 6369 6573 2077 6974 6820 666c  ndencies with fl
+00000c20: 6173 6b2d 6f70 656e 6170 6933 3a0d 0a0d  ask-openapi3:...
+00000c30: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
+00000c40: 7374 616c 6c20 666c 6173 6b2d 6f70 656e  stall flask-open
+00000c50: 6170 6933 5b79 616d 6c5d 0d0a 2320 6f72  api3[yaml]..# or
+00000c60: 0d0a 7069 7020 696e 7374 616c 6c20 666c  ..pip install fl
+00000c70: 6173 6b2d 6f70 656e 6170 6933 5b61 7379  ask-openapi3[asy
+00000c80: 6e63 5d0d 0a23 206f 720d 0a70 6970 2069  nc]..# or..pip i
+00000c90: 6e73 7461 6c6c 2066 6c61 736b 2d6f 7065  nstall flask-ope
+00000ca0: 6e61 7069 335b 646f 7465 6e76 5d0d 0a23  napi3[dotenv]..#
+00000cb0: 206f 720d 0a70 6970 2069 6e73 7461 6c6c   or..pip install
+00000cc0: 2066 6c61 736b 2d6f 7065 6e61 7069 335b   flask-openapi3[
+00000cd0: 656d 6169 6c5d 0d0a 2320 6f72 2061 6c6c  email]..# or all
+00000ce0: 0d0a 7069 7020 696e 7374 616c 6c20 666c  ..pip install fl
+00000cf0: 6173 6b2d 6f70 656e 6170 6933 5b79 616d  ask-openapi3[yam
+00000d00: 6c2c 6173 796e 632c 646f 7465 6e76 2c65  l,async,dotenv,e
+00000d10: 6d61 696c 5d0d 0a23 206f 7220 6d61 6e75  mail]..# or manu
+00000d20: 616c 6c79 0d0a 7069 7020 696e 7374 616c  ally..pip instal
+00000d30: 6c20 7079 7961 6d6c 2061 7367 6972 6566  l pyyaml asgiref
+00000d40: 2070 7974 686f 6e2d 646f 7465 6e76 2065   python-dotenv e
+00000d50: 6d61 696c 2d76 616c 6964 6174 6f72 0d0a  mail-validator..
+00000d60: 6060 600d 0a3c 2f64 6574 6169 6c73 3e0d  ```..</details>.
+00000d70: 0a0d 0a23 2320 4120 5369 6d70 6c65 2045  ...## A Simple E
+00000d80: 7861 6d70 6c65 0d0a 0d0a 4865 7265 2773  xample....Here's
+00000d90: 2061 2073 696d 706c 6520 6578 616d 706c   a simple exampl
+00000da0: 652c 2066 7572 7468 6572 2067 6f20 746f  e, further go to
+00000db0: 2074 6865 205b 4578 616d 706c 655d 2868   the [Example](h
+00000dc0: 7474 7073 3a2f 2f6c 756f 6c69 6e67 6368  ttps://luolingch
+00000dd0: 756e 2e67 6974 6875 622e 696f 2f66 6c61  un.github.io/fla
+00000de0: 736b 2d6f 7065 6e61 7069 332f 6c61 7465  sk-openapi3/late
+00000df0: 7374 2f45 7861 6d70 6c65 2f29 2e0d 0a0d  st/Example/)....
+00000e00: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00000e10: 2070 7964 616e 7469 6320 696d 706f 7274   pydantic import
+00000e20: 2042 6173 654d 6f64 656c 0d0a 0d0a 6672   BaseModel....fr
+00000e30: 6f6d 2066 6c61 736b 5f6f 7065 6e61 7069  om flask_openapi
+00000e40: 3320 696d 706f 7274 2049 6e66 6f2c 2054  3 import Info, T
+00000e50: 6167 0d0a 6672 6f6d 2066 6c61 736b 5f6f  ag..from flask_o
+00000e60: 7065 6e61 7069 3320 696d 706f 7274 204f  penapi3 import O
+00000e70: 7065 6e41 5049 0d0a 0d0a 696e 666f 203d  penAPI....info =
+00000e80: 2049 6e66 6f28 7469 746c 653d 2262 6f6f   Info(title="boo
+00000e90: 6b20 4150 4922 2c20 7665 7273 696f 6e3d  k API", version=
+00000ea0: 2231 2e30 2e30 2229 0d0a 6170 7020 3d20  "1.0.0")..app = 
+00000eb0: 4f70 656e 4150 4928 5f5f 6e61 6d65 5f5f  OpenAPI(__name__
+00000ec0: 2c20 696e 666f 3d69 6e66 6f29 0d0a 0d0a  , info=info)....
+00000ed0: 626f 6f6b 5f74 6167 203d 2054 6167 286e  book_tag = Tag(n
+00000ee0: 616d 653d 2262 6f6f 6b22 2c20 6465 7363  ame="book", desc
+00000ef0: 7269 7074 696f 6e3d 2253 6f6d 6520 426f  ription="Some Bo
+00000f00: 6f6b 2229 0d0a 0d0a 0d0a 636c 6173 7320  ok")......class 
+00000f10: 426f 6f6b 5175 6572 7928 4261 7365 4d6f  BookQuery(BaseMo
+00000f20: 6465 6c29 3a0d 0a20 2020 2061 6765 3a20  del):..    age: 
+00000f30: 696e 740d 0a20 2020 2061 7574 686f 723a  int..    author:
+00000f40: 2073 7472 0d0a 0d0a 0d0a 4061 7070 2e67   str......@app.g
+00000f50: 6574 2822 2f62 6f6f 6b22 2c20 7375 6d6d  et("/book", summ
+00000f60: 6172 793d 2267 6574 2062 6f6f 6b73 222c  ary="get books",
+00000f70: 2074 6167 733d 5b62 6f6f 6b5f 7461 675d   tags=[book_tag]
+00000f80: 290d 0a64 6566 2067 6574 5f62 6f6f 6b28  )..def get_book(
+00000f90: 7175 6572 793a 2042 6f6f 6b51 7565 7279  query: BookQuery
+00000fa0: 293a 0d0a 2020 2020 2222 220d 0a20 2020  ):..    """..   
+00000fb0: 2074 6f20 6765 7420 616c 6c20 626f 6f6b   to get all book
+00000fc0: 730d 0a20 2020 2022 2222 0d0a 2020 2020  s..    """..    
+00000fd0: 7265 7475 726e 207b 0d0a 2020 2020 2020  return {..      
+00000fe0: 2020 2263 6f64 6522 3a20 302c 0d0a 2020    "code": 0,..  
+00000ff0: 2020 2020 2020 226d 6573 7361 6765 223a        "message":
+00001000: 2022 6f6b 222c 0d0a 2020 2020 2020 2020   "ok",..        
+00001010: 2264 6174 6122 3a20 5b0d 0a20 2020 2020  "data": [..     
+00001020: 2020 2020 2020 207b 2262 6964 223a 2031         {"bid": 1
+00001030: 2c20 2261 6765 223a 2071 7565 7279 2e61  , "age": query.a
+00001040: 6765 2c20 2261 7574 686f 7222 3a20 7175  ge, "author": qu
+00001050: 6572 792e 6175 7468 6f72 7d2c 0d0a 2020  ery.author},..  
+00001060: 2020 2020 2020 2020 2020 7b22 6269 6422            {"bid"
+00001070: 3a20 322c 2022 6167 6522 3a20 7175 6572  : 2, "age": quer
+00001080: 792e 6167 652c 2022 6175 7468 6f72 223a  y.age, "author":
+00001090: 2071 7565 7279 2e61 7574 686f 727d 0d0a   query.author}..
+000010a0: 2020 2020 2020 2020 5d0d 0a20 2020 207d          ]..    }
+000010b0: 0d0a 0d0a 0d0a 6966 205f 5f6e 616d 655f  ......if __name_
+000010c0: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+000010d0: 0d0a 2020 2020 6170 702e 7275 6e28 6465  ..    app.run(de
+000010e0: 6275 673d 5472 7565 290d 0a60 6060 0d0a  bug=True)..```..
+000010f0: 0d0a 3c64 6574 6169 6c73 3e0d 0a3c 7375  ..<details>..<su
+00001100: 6d6d 6172 793e 436c 6173 732d 6261 7365  mmary>Class-base
+00001110: 6420 4150 4920 5669 6577 2045 7861 6d70  d API View Examp
+00001120: 6c65 3c2f 7375 6d6d 6172 793e 0d0a 0d0a  le</summary>....
+00001130: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00001140: 7479 7069 6e67 2069 6d70 6f72 7420 4f70  typing import Op
+00001150: 7469 6f6e 616c 0d0a 0d0a 6672 6f6d 2070  tional....from p
+00001160: 7964 616e 7469 6320 696d 706f 7274 2042  ydantic import B
+00001170: 6173 654d 6f64 656c 2c20 4669 656c 640d  aseModel, Field.
+00001180: 0a0d 0a66 726f 6d20 666c 6173 6b5f 6f70  ...from flask_op
+00001190: 656e 6170 6933 2069 6d70 6f72 7420 4f70  enapi3 import Op
+000011a0: 656e 4150 492c 2054 6167 2c20 496e 666f  enAPI, Tag, Info
+000011b0: 2c20 4150 4956 6965 770d 0a0d 0a0d 0a69  , APIView......i
+000011c0: 6e66 6f20 3d20 496e 666f 2874 6974 6c65  nfo = Info(title
+000011d0: 3d27 626f 6f6b 2041 5049 272c 2076 6572  ='book API', ver
+000011e0: 7369 6f6e 3d27 312e 302e 3027 290d 0a61  sion='1.0.0')..a
+000011f0: 7070 203d 204f 7065 6e41 5049 285f 5f6e  pp = OpenAPI(__n
+00001200: 616d 655f 5f2c 2069 6e66 6f3d 696e 666f  ame__, info=info
+00001210: 290d 0a0d 0a61 7069 5f76 6965 7720 3d20  )....api_view = 
+00001220: 4150 4956 6965 7728 7572 6c5f 7072 6566  APIView(url_pref
+00001230: 6978 3d22 2f61 7069 2f76 3122 2c20 7669  ix="/api/v1", vi
+00001240: 6577 5f74 6167 733d 5b54 6167 286e 616d  ew_tags=[Tag(nam
+00001250: 653d 2262 6f6f 6b22 295d 290d 0a0d 0a0d  e="book")]).....
+00001260: 0a63 6c61 7373 2042 6f6f 6b50 6174 6828  .class BookPath(
+00001270: 4261 7365 4d6f 6465 6c29 3a0d 0a20 2020  BaseModel):..   
+00001280: 2069 643a 2069 6e74 203d 2046 6965 6c64   id: int = Field
+00001290: 282e 2e2e 2c20 6465 7363 7269 7074 696f  (..., descriptio
+000012a0: 6e3d 2262 6f6f 6b20 4944 2229 0d0a 0d0a  n="book ID")....
+000012b0: 0d0a 636c 6173 7320 426f 6f6b 5175 6572  ..class BookQuer
+000012c0: 7928 4261 7365 4d6f 6465 6c29 3a0d 0a20  y(BaseModel):.. 
+000012d0: 2020 2061 6765 3a20 4f70 7469 6f6e 616c     age: Optional
+000012e0: 5b69 6e74 5d20 3d20 4669 656c 6428 4e6f  [int] = Field(No
+000012f0: 6e65 2c20 6465 7363 7269 7074 696f 6e3d  ne, description=
+00001300: 2741 6765 2729 0d0a 0d0a 0d0a 636c 6173  'Age')......clas
+00001310: 7320 426f 6f6b 426f 6479 2842 6173 654d  s BookBody(BaseM
+00001320: 6f64 656c 293a 0d0a 2020 2020 6167 653a  odel):..    age:
+00001330: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00001340: 2046 6965 6c64 282e 2e2e 2c20 6765 3d32   Field(..., ge=2
+00001350: 2c20 6c65 3d34 2c20 6465 7363 7269 7074  , le=4, descript
+00001360: 696f 6e3d 2741 6765 2729 0d0a 2020 2020  ion='Age')..    
+00001370: 6175 7468 6f72 3a20 7374 7220 3d20 4669  author: str = Fi
+00001380: 656c 6428 4e6f 6e65 2c20 6d69 6e5f 6c65  eld(None, min_le
+00001390: 6e67 7468 3d32 2c20 6d61 785f 6c65 6e67  ngth=2, max_leng
+000013a0: 7468 3d34 2c20 6465 7363 7269 7074 696f  th=4, descriptio
+000013b0: 6e3d 2741 7574 686f 7227 290d 0a0d 0a0d  n='Author').....
+000013c0: 0a40 6170 695f 7669 6577 2e72 6f75 7465  .@api_view.route
+000013d0: 2822 2f62 6f6f 6b22 290d 0a63 6c61 7373  ("/book")..class
+000013e0: 2042 6f6f 6b4c 6973 7441 5049 5669 6577   BookListAPIView
+000013f0: 3a0d 0a20 2020 2061 203d 2031 0d0a 0d0a  :..    a = 1....
+00001400: 2020 2020 4061 7069 5f76 6965 772e 646f      @api_view.do
+00001410: 6328 7375 6d6d 6172 793d 2267 6574 2062  c(summary="get b
+00001420: 6f6f 6b20 6c69 7374 2229 0d0a 2020 2020  ook list")..    
+00001430: 6465 6620 6765 7428 7365 6c66 2c20 7175  def get(self, qu
+00001440: 6572 793a 2042 6f6f 6b51 7565 7279 293a  ery: BookQuery):
+00001450: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00001460: 7365 6c66 2e61 290d 0a20 2020 2020 2020  self.a)..       
+00001470: 2072 6574 7572 6e20 7175 6572 792e 6d6f   return query.mo
+00001480: 6465 6c5f 6475 6d70 5f6a 736f 6e28 290d  del_dump_json().
+00001490: 0a0d 0a20 2020 2040 6170 695f 7669 6577  ...    @api_view
+000014a0: 2e64 6f63 2873 756d 6d61 7279 3d22 6372  .doc(summary="cr
+000014b0: 6561 7465 2062 6f6f 6b22 290d 0a20 2020  eate book")..   
+000014c0: 2064 6566 2070 6f73 7428 7365 6c66 2c20   def post(self, 
+000014d0: 626f 6479 3a20 426f 6f6b 426f 6479 293a  body: BookBody):
+000014e0: 0d0a 2020 2020 2020 2020 2222 2264 6573  ..        """des
+000014f0: 6372 6970 7469 6f6e 2066 6f72 2061 2063  cription for a c
+00001500: 7265 6174 6564 2062 6f6f 6b22 2222 0d0a  reated book"""..
+00001510: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00001520: 6f64 792e 6d6f 6465 6c5f 6475 6d70 5f6a  ody.model_dump_j
+00001530: 736f 6e28 290d 0a0d 0a0d 0a40 6170 695f  son()......@api_
+00001540: 7669 6577 2e72 6f75 7465 2822 2f62 6f6f  view.route("/boo
+00001550: 6b2f 3c69 643e 2229 0d0a 636c 6173 7320  k/<id>")..class 
+00001560: 426f 6f6b 4150 4956 6965 773a 0d0a 2020  BookAPIView:..  
+00001570: 2020 4061 7069 5f76 6965 772e 646f 6328    @api_view.doc(
+00001580: 7375 6d6d 6172 793d 2267 6574 2062 6f6f  summary="get boo
+00001590: 6b22 290d 0a20 2020 2064 6566 2067 6574  k")..    def get
+000015a0: 2873 656c 662c 2070 6174 683a 2042 6f6f  (self, path: Boo
+000015b0: 6b50 6174 6829 3a0d 0a20 2020 2020 2020  kPath):..       
+000015c0: 2070 7269 6e74 2870 6174 6829 0d0a 2020   print(path)..  
+000015d0: 2020 2020 2020 7265 7475 726e 2022 6765        return "ge
+000015e0: 7422 0d0a 0d0a 2020 2020 4061 7069 5f76  t"....    @api_v
+000015f0: 6965 772e 646f 6328 7375 6d6d 6172 793d  iew.doc(summary=
+00001600: 2275 7064 6174 6520 626f 6f6b 2229 0d0a  "update book")..
+00001610: 2020 2020 6465 6620 7075 7428 7365 6c66      def put(self
+00001620: 2c20 7061 7468 3a20 426f 6f6b 5061 7468  , path: BookPath
+00001630: 293a 0d0a 2020 2020 2020 2020 7072 696e  ):..        prin
+00001640: 7428 7061 7468 290d 0a20 2020 2020 2020  t(path)..       
+00001650: 2072 6574 7572 6e20 2270 7574 220d 0a0d   return "put"...
+00001660: 0a20 2020 2040 6170 695f 7669 6577 2e64  .    @api_view.d
+00001670: 6f63 2873 756d 6d61 7279 3d22 6465 6c65  oc(summary="dele
+00001680: 7465 2062 6f6f 6b22 2c20 6465 7072 6563  te book", deprec
+00001690: 6174 6564 3d54 7275 6529 0d0a 2020 2020  ated=True)..    
+000016a0: 6465 6620 6465 6c65 7465 2873 656c 662c  def delete(self,
+000016b0: 2070 6174 683a 2042 6f6f 6b50 6174 6829   path: BookPath)
+000016c0: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+000016d0: 2870 6174 6829 0d0a 2020 2020 2020 2020  (path)..        
+000016e0: 7265 7475 726e 2022 6465 6c65 7465 220d  return "delete".
+000016f0: 0a0d 0a0d 0a61 7070 2e72 6567 6973 7465  .....app.registe
+00001700: 725f 6170 695f 7669 6577 2861 7069 5f76  r_api_view(api_v
+00001710: 6965 7729 0d0a 0d0a 6966 205f 5f6e 616d  iew)....if __nam
+00001720: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
+00001730: 223a 0d0a 2020 2020 6170 702e 7275 6e28  ":..    app.run(
+00001740: 6465 6275 673d 5472 7565 290d 0a60 6060  debug=True)..```
+00001750: 0d0a 3c2f 6465 7461 696c 733e 0d0a 0d0a  ..</details>....
+00001760: 2323 2041 5049 2044 6f63 756d 656e 740d  ## API Document.
+00001770: 0a0d 0a52 756e 2074 6865 205b 7369 6d70  ...Run the [simp
+00001780: 6c65 2065 7861 6d70 6c65 5d28 6874 7470  le example](http
+00001790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+000017a0: 756f 6c69 6e67 6368 756e 2f66 6c61 736b  uolingchun/flask
+000017b0: 2d6f 7065 6e61 7069 332f 626c 6f62 2f6d  -openapi3/blob/m
+000017c0: 6173 7465 722f 6578 616d 706c 6573 2f73  aster/examples/s
+000017d0: 696d 706c 655f 6465 6d6f 2e70 7929 2c20  imple_demo.py), 
+000017e0: 616e 6420 676f 2074 6f20 6874 7470 3a2f  and go to http:/
+000017f0: 2f31 3237 2e30 2e30 2e31 3a35 3030 302f  /127.0.0.1:5000/
+00001800: 6f70 656e 6170 692e 0d0a 0d0a 596f 7520  openapi.....You 
+00001810: 7769 6c6c 2073 6565 2074 6865 2064 6f63  will see the doc
+00001820: 756d 656e 7461 7469 6f6e 3a20 5b53 7761  umentation: [Swa
+00001830: 6767 6572 5d28 6874 7470 733a 2f2f 6769  gger](https://gi
+00001840: 7468 7562 2e63 6f6d 2f73 7761 6767 6572  thub.com/swagger
+00001850: 2d61 7069 2f73 7761 6767 6572 2d75 6929  -api/swagger-ui)
+00001860: 2c20 5b52 6564 6f63 5d28 6874 7470 733a  , [Redoc](https:
+00001870: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6564  //github.com/Red
+00001880: 6f63 6c79 2f72 6564 6f63 2920 616e 6420  ocly/redoc) and 
+00001890: 5b52 6170 6944 6f63 5d28 6874 7470 733a  [RapiDoc](https:
+000018a0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6170  //github.com/rap
+000018b0: 692d 646f 632f 5261 7069 446f 6329 2e0d  i-doc/RapiDoc)..
+000018c0: 0a0d 0a3e 2053 7761 6767 6572 2c20 5265  ...> Swagger, Re
+000018d0: 646f 632c 2052 6170 6944 6f63 2061 7265  doc, RapiDoc are
+000018e0: 206f 7074 696f 6e61 6c20 6465 7065 6e64   optional depend
+000018f0: 656e 6369 6573 2074 6861 7420 7265 7175  encies that requ
+00001900: 6972 6520 6d61 6e75 616c 2069 6e73 7461  ire manual insta
+00001910: 6c6c 6174 696f 6e2e 0d0a 3e0d 0a3e 2060  llation...>..> `
+00001920: 7069 7020 696e 7374 616c 6c20 2d55 2066  pip install -U f
+00001930: 6c61 736b 2d6f 7065 6e61 7069 335b 7377  lask-openapi3[sw
+00001940: 6167 6765 722c 7265 646f 632c 7261 7069  agger,redoc,rapi
+00001950: 646f 635d 600d 0a3e 200d 0a3e 204d 6f72  doc]`..> ..> Mor
+00001960: 6520 6f70 7469 6f6e 616c 2075 6920 7465  e optional ui te
+00001970: 6d70 6c61 7465 7320 676f 746f 2074 6865  mplates goto the
+00001980: 2064 6f63 756d 656e 7420 6162 6f75 7420   document about 
+00001990: 5b55 495f 5465 6d70 6c61 7465 735d 2868  [UI_Templates](h
+000019a0: 7474 7073 3a2f 2f6c 756f 6c69 6e67 6368  ttps://luolingch
+000019b0: 756e 2e67 6974 6875 622e 696f 2f66 6c61  un.github.io/fla
+000019c0: 736b 2d6f 7065 6e61 7069 332f 6c61 7465  sk-openapi3/late
+000019d0: 7374 2f55 7361 6765 2f55 495f 5465 6d70  st/Usage/UI_Temp
+000019e0: 6c61 7465 732f 292e 0d0a 0d0a 215b 6f70  lates/).....![op
+000019f0: 656e 6170 695d 2868 7474 7073 3a2f 2f72  enapi](https://r
+00001a00: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00001a10: 7465 6e74 2e63 6f6d 2f6c 756f 6c69 6e67  tent.com/luoling
+00001a20: 6368 756e 2f66 6c61 736b 2d6f 7065 6e61  chun/flask-opena
+00001a30: 7069 332f 6d61 7374 6572 2f64 6f63 732f  pi3/master/docs/
+00001a40: 696d 6167 6573 2f6f 7065 6e61 7069 2e70  images/openapi.p
+00001a50: 6e67 290d 0a21 5b6f 7065 6e61 7069 2d73  ng)..![openapi-s
+00001a60: 7761 6767 6572 5d28 6874 7470 733a 2f2f  wagger](https://
+00001a70: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00001a80: 6e74 656e 742e 636f 6d2f 6c75 6f6c 696e  ntent.com/luolin
+00001a90: 6763 6875 6e2f 666c 6173 6b2d 6f70 656e  gchun/flask-open
+00001aa0: 6170 6933 2f6d 6173 7465 722f 646f 6373  api3/master/docs
+00001ab0: 2f69 6d61 6765 732f 6f70 656e 6170 692d  /images/openapi-
+00001ac0: 7377 6167 6765 722e 706e 6729 0d0a 215b  swagger.png)..![
+00001ad0: 6f70 656e 6170 692d 7265 646f 635d 2868  openapi-redoc](h
+00001ae0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001af0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001b00: 2f6c 756f 6c69 6e67 6368 756e 2f66 6c61  /luolingchun/fla
+00001b10: 736b 2d6f 7065 6e61 7069 332f 6d61 7374  sk-openapi3/mast
+00001b20: 6572 2f64 6f63 732f 696d 6167 6573 2f6f  er/docs/images/o
+00001b30: 7065 6e61 7069 2d72 6564 6f63 2e70 6e67  penapi-redoc.png
+00001b40: 290d 0a21 5b6f 7065 6e61 7069 2d52 6170  )..![openapi-Rap
+00001b50: 6944 6f63 5d28 6874 7470 733a 2f2f 7261  iDoc](https://ra
+00001b60: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00001b70: 656e 742e 636f 6d2f 6c75 6f6c 696e 6763  ent.com/luolingc
+00001b80: 6875 6e2f 666c 6173 6b2d 6f70 656e 6170  hun/flask-openap
+00001b90: 6933 2f6d 6173 7465 722f 646f 6373 2f69  i3/master/docs/i
+00001ba0: 6d61 6765 732f 6f70 656e 6170 692d 7261  mages/openapi-ra
+00001bb0: 7069 646f 632e 706e 6729 0d0a            pidoc.png)..
```

### Comparing `flask_openapi3-3.1.1/pyproject.toml` & `flask_openapi3-4.0.0.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,84 @@
-[project]
-name = "flask-openapi3"
-description = "Generate REST API and OpenAPI documentation for your Flask project."
-readme = "README.md"
-license = { text = "MIT" }
-maintainers = [{ name = "llc", email = "luolingchun@outlook.com" }]
-classifiers = [
-    # "Development Status :: 1 - Planning",
-    # "Development Status :: 2 - Pre-Alpha",
-    # "Development Status :: 3 - Alpha",
-    # "Development Status :: 4 - Beta",
-    "Development Status :: 5 - Production/Stable",
-    # "Development Status :: 6 - Mature",
-    # "Development Status :: 7 - Inactive",
-    "Environment :: Web Environment",
-    "Framework :: Flask",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-]
-requires-python = ">=3.8"
-dependencies = ["Flask>=2.0", "pydantic>=2.4"]
-dynamic = ["version"]
-
-[project.urls]
-Homepage = "https://github.com/luolingchun/flask-openapi3"
-Documentation = "https://luolingchun.github.io/flask-openapi3"
-
-[project.optional-dependencies]
-yaml = ["pyyaml"]
-async = ["asgiref >= 3.2"]
-dotenv = ["python-dotenv"]
-email = ["email-validator"]
-
-
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch.version]
-path = "flask_openapi3/__version__.py"
-
-[tool.hatch.build.targets.sdist]
-include = [
-    "/flask_openapi3",
-    "/examples",
-    "/requirements",
-    "/tests",
-    "/CHANGELOG.md",
-    "/CONTRIBUTING.md",
-    "/LICENSE.rst"
-]
-
-
-[tool.flake8]
-per-file-ignores = ["__init__.py:F401"]
-max-line-length = 120
-count = true
-
-
-[tool.mypy]
-files = "src"
-plugins = ["pydantic.mypy"]
-
-[[tool.mypy.overrides]]
-module = ["pydantic_core.*", "devtools.*"]
-follow_imports = "skip"
-ignore_missing_imports = true
-
+[project]
+name = "flask-openapi3"
+description = "Generate REST API and OpenAPI documentation for your Flask project."
+readme = "README.md"
+license = { text = "MIT" }
+maintainers = [{ name = "llc", email = "luolingchun@outlook.com" }]
+classifiers = [
+    # "Development Status :: 1 - Planning",
+    # "Development Status :: 2 - Pre-Alpha",
+    # "Development Status :: 3 - Alpha",
+    # "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
+    # "Development Status :: 6 - Mature",
+    # "Development Status :: 7 - Inactive",
+    "Environment :: Web Environment",
+    "Framework :: Flask",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+requires-python = ">=3.8"
+dependencies = ["Flask>=2.0", "pydantic>=2.4"]
+dynamic = ["version"]
+
+[project.urls]
+Homepage = "https://github.com/luolingchun/flask-openapi3"
+Documentation = "https://luolingchun.github.io/flask-openapi3"
+
+[project.optional-dependencies]
+yaml = ["pyyaml"]
+async = ["asgiref >= 3.2"]
+dotenv = ["python-dotenv"]
+email = ["email-validator"]
+# ui templates
+swagger = ["flask-openapi3-swagger"]
+redoc = ["flask-openapi3-redoc"]
+rapidoc = ["flask-openapi3-rapidoc"]
+rapipdf = ["flask-openapi3-rapipdf"]
+scalar = ["flask-openapi3-scalar"]
+elements = ["flask-openapi3-elements"]
+
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.hatch.version]
+path = "flask_openapi3/__version__.py"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/flask_openapi3",
+    "/examples",
+    "/requirements",
+    "/tests",
+    "/CHANGELOG.md",
+    "/CONTRIBUTING.md",
+    "/LICENSE.rst"
+]
+
+
+[tool.flake8]
+per-file-ignores = ["__init__.py:F401"]
+max-line-length = 120
+count = true
+
+
+[tool.mypy]
+files = "src"
+plugins = ["pydantic.mypy"]
+
+[[tool.mypy.overrides]]
+module = ["pydantic_core.*", "devtools.*"]
+follow_imports = "skip"
+ignore_missing_imports = true
+
```

### Comparing `flask_openapi3-3.1.1/PKG-INFO` & `flask_openapi3-4.0.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flask-openapi3
-Version: 3.1.1
+Version: 4.0.0.dev0
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Project-URL: Homepage, https://github.com/luolingchun/flask-openapi3
 Project-URL: Documentation, https://luolingchun.github.io/flask-openapi3
 Maintainer-email: llc <luolingchun@outlook.com>
 License: MIT
 License-File: LICENSE.rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,28 @@
 Requires-Python: >=3.8
 Requires-Dist: flask>=2.0
 Requires-Dist: pydantic>=2.4
 Provides-Extra: async
 Requires-Dist: asgiref>=3.2; extra == 'async'
 Provides-Extra: dotenv
 Requires-Dist: python-dotenv; extra == 'dotenv'
+Provides-Extra: elements
+Requires-Dist: flask-openapi3-elements; extra == 'elements'
 Provides-Extra: email
 Requires-Dist: email-validator; extra == 'email'
+Provides-Extra: rapidoc
+Requires-Dist: flask-openapi3-rapidoc; extra == 'rapidoc'
+Provides-Extra: rapipdf
+Requires-Dist: flask-openapi3-rapipdf; extra == 'rapipdf'
+Provides-Extra: redoc
+Requires-Dist: flask-openapi3-redoc; extra == 'redoc'
+Provides-Extra: scalar
+Requires-Dist: flask-openapi3-scalar; extra == 'scalar'
+Provides-Extra: swagger
+Requires-Dist: flask-openapi3-swagger; extra == 'swagger'
 Provides-Extra: yaml
 Requires-Dist: pyyaml; extra == 'yaml'
 Description-Content-Type: text/markdown
 
 <div align="center">
     <a href="https://luolingchun.github.io/flask-openapi3/" target="_blank">
         <img class="off-glb" src="https://raw.githubusercontent.com/luolingchun/flask-openapi3/master/docs/images/logo-text.svg" 
@@ -54,24 +66,26 @@
         <img class="off-glb" src="https://img.shields.io/pypi/dm/flask-openapi3" alt="pypistats">
     </a>
     <a href="https://pypi.org/project/flask-openapi3/" target="_blank">
         <img class="off-glb" src="https://img.shields.io/pypi/pyversions/flask-openapi3" alt="pypi versions">
     </a>
 </p>
 
+> This branch is in development preview state.
+
 **Flask OpenAPI3** is a web API framework based on **Flask**. It uses **Pydantic** to verify data and automatic
-generation of interaction documentation: **Swagger**, **ReDoc** and **RapiDoc**.
+generation of interaction documentation: **Swagger**, **ReDoc**, **RapiDoc**, etc.
 
 The key features are:
 
 - **Easy to code:** Easy to use and easy to learn
 
 - **Standard document specification:** Based on [OpenAPI Specification](https://spec.openapis.org/oas/v3.1.0)
 
-- **Interactive OpenAPI documentation:** [Swagger](https://github.com/swagger-api/swagger-ui), [Redoc](https://github.com/Redocly/redoc) and [RapiDoc](https://github.com/rapi-doc/RapiDoc)
+- **Interactive OpenAPI documentation:** [Swagger](https://github.com/swagger-api/swagger-ui), [Redoc](https://github.com/Redocly/redoc), [RapiDoc](https://github.com/rapi-doc/RapiDoc), etc.
   
 - **Data validation:** Fast data verification based on [Pydantic](https://github.com/pydantic/pydantic)
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
 ## Requirements
 
@@ -81,21 +95,21 @@
 
 - [Flask](https://github.com/pallets/flask) for the web app.
 - [Pydantic](https://github.com/pydantic/pydantic) for the data validation.
 
 ## Installation
 
 ```bash
-pip install -U flask-openapi3
+pip install -U flask-openapi3[swagger]
 ```
 
 or
 
 ```bash
-conda install -c conda-forge flask-openapi3
+conda install -c conda-forge flask-openapi3[swagger]
 ```
 
 <details markdown="block">
 <summary>Optional dependencies</summary>
 
 - [python-email-validator](https://github.com/JoshData/python-email-validator) supports email verification.
 - [python-dotenv](https://github.com/theskumar/python-dotenv#readme) enables support for [Environment Variables From dotenv](https://flask.palletsprojects.com/en/latest/cli/#dotenv) when running `flask` commands.
@@ -231,11 +245,17 @@
 
 ## API Document
 
 Run the [simple example](https://github.com/luolingchun/flask-openapi3/blob/master/examples/simple_demo.py), and go to http://127.0.0.1:5000/openapi.
 
 You will see the documentation: [Swagger](https://github.com/swagger-api/swagger-ui), [Redoc](https://github.com/Redocly/redoc) and [RapiDoc](https://github.com/rapi-doc/RapiDoc).
 
+> Swagger, Redoc, RapiDoc are optional dependencies that require manual installation.
+>
+> `pip install -U flask-openapi3[swagger,redoc,rapidoc]`
+> 
+> More optional ui templates goto the document about [UI_Templates](https://luolingchun.github.io/flask-openapi3/latest/Usage/UI_Templates/).
+
 ![openapi](https://raw.githubusercontent.com/luolingchun/flask-openapi3/master/docs/images/openapi.png)
 ![openapi-swagger](https://raw.githubusercontent.com/luolingchun/flask-openapi3/master/docs/images/openapi-swagger.png)
 ![openapi-redoc](https://raw.githubusercontent.com/luolingchun/flask-openapi3/master/docs/images/openapi-redoc.png)
 ![openapi-RapiDoc](https://raw.githubusercontent.com/luolingchun/flask-openapi3/master/docs/images/openapi-rapidoc.png)
```

