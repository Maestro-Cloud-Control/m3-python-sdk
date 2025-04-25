# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.1] 2025-04-25
### Changes:
- Update the `delete_consumption` method in the `ConsumptionResource` class 
to make the `target_region` parameter optional

## [1.1.0] 2024-09-18
### Changes:
- Update `pika` library from version `1.0.0b1` to `1.3.2`
- Update `RabbitMqStrategy` class to support `pika` version `1.3.2`
- Update `pyproject.toml`
- Remove `setup.cfg` and `setup.py`
- Update from `uuid1` to `uuid4`
- Add unit tests for `RabbitMqStrategy` class
- Add unit tests for `HttpStrategy` class
- Add `AdjustmentApiActions` and `ConsumptionApiActions` classes to group API 
action constants. Update usage of API action constants in client execution calls
- Update: Move `CHECK_TENANT_STATUS` and `GET_TOTAL_BILLING_REPORT` constants to
`BillingApiActions` class

## [1.0.7] 2024-02-27
### Added
- Ability to send batch requests
- Methods: `post_process_batch_request`,  `execute_batch`,`execute_batch_async`,
`_build_request`, `_build_secure_request`, `pre_process_batch_request`,
`execute_batch_sync`, `add_consumption_batch`, `build_consumption_params`

## [1.0.6] 2023-12-08
### Added
- Missing headers for `execute_async` method
- Headers logs for `execute_sync`, `execute_async` methods

## [1.0.5] 2023-12-07

### Added
- Rabbit options logs for `execute_async` method

### Changed
- `content_type` for `execute_async` method from `application/json` to `text/plain`

## [1.0.4] 2023-12-06

### Added
- RabbitMQ `request_queue`, `response_queue`, `exchange` values logging

## [1.0.3] 2023-12-01

### Changed
- Response format changed, for failed checks if response is json type

## [1.0.2] 2023-11-29

### Changed
- Response format changed, few params deleted from response
- setup.cfg updated, the way of installing `cryptography` changed, `botocore` deleted 

## [1.0.1] 2023-11-27

### Added
- Root logger name `python_sdk`

### Removed
- Root logger level setting

## [1.0.0] 2023-11-23

### Added
- RabbitMQ and HTTP transport functionality.
- Billing resource with following methods:
    - `describe_billing_month`
    - `get_currency`
    - `get_top_accounts_report`
    - `add_cost_center`
    - `billing_configure`
    - `archive_big_query`
- Adjustment resource with following methods:
    - `add_adjustment`
    - `get_adjustment`
    - `delete_adjustment`
    - `total_report`
- Consumption resource with following methods:
    - `add_consumption`
    - `get_consumption`
    - `delete_consumption`
    - `add_consumption_details`
    - `get_consumption_details`
    - `delete_consumption_details`
    - `check_tenant_status`


   
