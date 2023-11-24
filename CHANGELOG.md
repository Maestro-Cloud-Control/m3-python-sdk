# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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


   
