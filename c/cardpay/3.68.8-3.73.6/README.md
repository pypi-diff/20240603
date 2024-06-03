# Comparing `tmp/cardpay-3.68.8.tar.gz` & `tmp/cardpay-3.73.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cardpay-3.68.8.tar", last modified: Thu Apr 18 09:30:27 2024, max compression
+gzip compressed data, was "dist/cardpay-3.73.6.tar", last modified: Mon Jun  3 06:12:56 2024, max compression
```

## Comparing `cardpay-3.68.8.tar` & `cardpay-3.73.6.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:30:27.000000 cardpay-3.68.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay/api/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5123 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     7288 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/authentication_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4229 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/card_info_api.py
--rw-rw-rw-   0 root         (0) root         (0)     7167 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/invoices_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3585 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/limits_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4356 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/mobile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37159 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/payments_api.py
--rw-rw-rw-   0 root         (0) root         (0)    18944 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/payouts_api.py
--rw-rw-rw-   0 root         (0) root         (0)     7344 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/pix_account_details_api.py
--rw-rw-rw-   0 root         (0) root         (0)    66001 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/recurrings_api.py
--rw-rw-rw-   0 root         (0) root         (0)    18934 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/refunds_api.py
--rw-rw-rw-   0 root         (0) root         (0)     9284 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api/reports_api_controller_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay/model/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5372 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/api_error.py
--rw-rw-rw-   0 root         (0) root         (0)     7379 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/api_tokens.py
--rw-rw-rw-   0 root         (0) root         (0)    18596 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/auth_data_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5092 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/authentication_create_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11735 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/authentication_customer.py
--rw-rw-rw-   0 root         (0) root         (0)    13558 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/authentication_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11482 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/authentication_data_request.py
--rw-rw-rw-   0 root         (0) root         (0)     8431 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/authentication_data_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/authentication_error.py
--rw-rw-rw-   0 root         (0) root         (0)     5713 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/bad_request_error.py
--rw-rw-rw-   0 root         (0) root         (0)    13721 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/bank_card_payout_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/billing_address.py
--rw-rw-rw-   0 root         (0) root         (0)    12881 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/browser_info.py
--rw-rw-rw-   0 root         (0) root         (0)     4303 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/card_info_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6868 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/card_info_response.py
--rw-rw-rw-   0 root         (0) root         (0)     9342 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/change_subscription_status_claim_response.py
--rw-rw-rw-   0 root         (0) root         (0)    10169 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/changed_plan_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/claim_response_subscription_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5510 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/confirm3ds_request.py
--rw-rw-rw-   0 root         (0) root         (0)     3720 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/device.py
--rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8018 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4637 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response_card.py
--rw-rw-rw-   0 root         (0) root         (0)     3846 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response_card_account.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response_customer.py
--rw-rw-rw-   0 root         (0) root         (0)    11765 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response_dispute_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4529 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)     8062 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/dispute_response_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7543 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/ewallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)    10758 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/filing_recurring_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12222 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/filing_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7186 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/filing_request_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)     4259 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/filing_request_subscription_data.py
--rw-rw-rw-   0 root         (0) root         (0)    13315 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/filter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10996 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/flight.py
--rw-rw-rw-   0 root         (0) root         (0)    17117 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/flights.py
--rw-rw-rw-   0 root         (0) root         (0)    20816 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/installment_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3692 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_creation_data_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_creation_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5456 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_customer.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8359 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_get_data_response.py
--rw-rw-rw-   0 root         (0) root         (0)     7069 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_get_response.py
--rw-rw-rw-   0 root         (0) root         (0)     6186 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_item.py
--rw-rw-rw-   0 root         (0) root         (0)     5102 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)     9015 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/invoice_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/item.py
--rw-rw-rw-   0 root         (0) root         (0)     4089 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/limit_info_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/mobile_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/mobile_token_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3862 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/next_subscription_payment.py
--rw-rw-rw-   0 root         (0) root         (0)     5681 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/not_found_error.py
--rw-rw-rw-   0 root         (0) root         (0)     4765 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/o_auth_error.py
--rw-rw-rw-   0 root         (0) root         (0)    22171 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/oneclick_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11846 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     8326 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_confirm3ds_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_execute_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_gateway_creation_response.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_gateway_response_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7526 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_increment_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6693 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_methods_response.py
--rw-rw-rw-   0 root         (0) root         (0)     6143 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_patch_request.py
--rw-rw-rw-   0 root         (0) root         (0)    14704 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request.py
--rw-rw-rw-   0 root         (0) root         (0)     9784 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_card.py
--rw-rw-rw-   0 root         (0) root         (0)    10524 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_card_account.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_cryptocurrency_account.py
--rw-rw-rw-   0 root         (0) root         (0)    24043 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_customer.py
--rw-rw-rw-   0 root         (0) root         (0)     9885 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_e_wallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)     8837 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_living_address.py
--rw-rw-rw-   0 root         (0) root         (0)    11036 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)    24815 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_request_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7973 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12115 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_response_card_account.py
--rw-rw-rw-   0 root         (0) root         (0)     7192 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_response_cryptocurrency_account.py
--rw-rw-rw-   0 root         (0) root         (0)    13026 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_response_customer.py
--rw-rw-rw-   0 root         (0) root         (0)    23247 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_response_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7466 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_update_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5410 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payment_update_transaction_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4577 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payments_list.py
--rw-rw-rw-   0 root         (0) root         (0)    12413 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_creation_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4248 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)    13066 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5485 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_card.py
--rw-rw-rw-   0 root         (0) root         (0)     7928 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_card_account.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_cryptocurrency_account.py
--rw-rw-rw-   0 root         (0) root         (0)    16987 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_customer.py
--rw-rw-rw-   0 root         (0) root         (0)    10769 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_e_wallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)     9023 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_living_address.py
--rw-rw-rw-   0 root         (0) root         (0)     6313 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)     9324 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_request_payout_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12397 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_response.py
--rw-rw-rw-   0 root         (0) root         (0)    10792 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_response_card_account.py
--rw-rw-rw-   0 root         (0) root         (0)     7076 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_response_cryptocurrency_account.py
--rw-rw-rw-   0 root         (0) root         (0)     7034 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_response_customer.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_response_e_wallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)    13951 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_response_payout_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4710 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/plan.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5117 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payout_update_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4560 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/payouts_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/pix_account_details_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4094 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/pix_account_details_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4583 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/plan_data_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6809 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/plan_quantity.py
--rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/plan_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6484 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/plan_update_request_plan_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3990 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/plan_update_response.py
--rw-rw-rw-   0 root         (0) root         (0)     9077 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     8431 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_confirm3ds_request.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_creation_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17547 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_customer.py
--rw-rw-rw-   0 root         (0) root         (0)     9245 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6621 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_execute_request.py
--rw-rw-rw-   0 root         (0) root         (0)    15170 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_filter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_gateway_creation_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5024 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_gateway_response_recurring_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7623 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_increment_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6219 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_patch_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_plan_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13848 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_plan_request_plan_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_plan_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4517 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_request_filing.py
--rw-rw-rw-   0 root         (0) root         (0)    27321 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_request_recurring_data.py
--rw-rw-rw-   0 root         (0) root         (0)     9166 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3936 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_response_filing.py
--rw-rw-rw-   0 root         (0) root         (0)     5115 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_response_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)    31219 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_response_recurring_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7563 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6612 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurring_update_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/recurrings_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/redirect_url_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11182 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     8960 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6959 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_request_customer.py
--rw-rw-rw-   0 root         (0) root         (0)     8267 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_request_e_wallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5521 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_request_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)     3893 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_request_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5103 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_request_refund_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10175 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_response.py
--rw-rw-rw-   0 root         (0) root         (0)     7961 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_response_card_account.py
--rw-rw-rw-   0 root         (0) root         (0)     6319 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_response_customer.py
--rw-rw-rw-   0 root         (0) root         (0)     3766 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_response_e_wallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)     4705 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_response_payment_data.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_response_refund_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5117 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refund_update_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4560 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/refunds_list.py
--rw-rw-rw-   0 root         (0) root         (0)    10169 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/renamed_plan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11448 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/report.py
--rw-rw-rw-   0 root         (0) root         (0)     6065 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/reports_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/reports_request.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/reports_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4597 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/request_updated_transaction_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12878 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/response_plan_data.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/response_updated_transaction_data.py
--rw-rw-rw-   0 root         (0) root         (0)     9586 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/return_urls.py
--rw-rw-rw-   0 root         (0) root         (0)    18412 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/scheduled_by_merchant_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19286 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/scheduled_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/shipping_address.py
--rw-rw-rw-   0 root         (0) root         (0)     3678 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription.py
--rw-rw-rw-   0 root         (0) root         (0)     4377 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_customer.py
--rw-rw-rw-   0 root         (0) root         (0)    17289 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_filter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    23206 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_get_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3664 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_get_response_plan.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_pending_plan_update.py
--rw-rw-rw-   0 root         (0) root         (0)     7366 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)     9092 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_update_request_subscription_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4061 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/subscription_update_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4393 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/supported_payment_method.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/three_d_secure_data.py
--rw-rw-rw-   0 root         (0) root         (0)    16067 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/three_d_secure_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5094 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/transaction_methods_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/transaction_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5407 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/transaction_response_e_wallet_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5105 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/transaction_response_merchant_order.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/transaction_update_request.py
--rw-rw-rw-   0 root         (0) root         (0)    10169 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/updated_plan_data.py
--rw-rw-rw-   0 root         (0) root         (0)    16550 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/updated_subscription_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5038 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/model/updated_subscription_recurring_data.py
--rw-rw-rw-   0 root         (0) root         (0)    14892 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32460 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     7335 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)    13856 2024-04-18 09:30:11.000000 cardpay-3.68.8/cardpay/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8129 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 09:30:27.000000 cardpay-3.68.8/cardpay.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-18 09:30:11.000000 cardpay-3.68.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     3600 2024-04-18 09:30:11.000000 cardpay-3.68.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-18 09:30:27.000000 cardpay-3.68.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-04-18 09:30:27.000000 cardpay-3.68.8/setup.py
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-18 09:30:27.000000 cardpay-3.68.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:12:56.000000 cardpay-3.73.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay/api/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7288 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/authentication_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4229 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/card_info_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7167 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/invoices_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3585 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/limits_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4356 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/mobile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37159 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/payments_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    18944 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/payouts_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7344 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/pix_account_details_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    66001 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/recurrings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    18934 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/refunds_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9284 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api/reports_api_controller_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay/model/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5372 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     7379 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/api_tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)    18596 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/auth_data_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5092 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/authentication_create_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11735 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/authentication_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/authentication_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11482 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/authentication_data_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     8431 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/authentication_data_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/authentication_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     5713 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/bad_request_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    13721 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/bank_card_payout_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/billing_address.py
+-rw-rw-rw-   0 root         (0) root         (0)    12881 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/browser_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/card_info_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6868 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/card_info_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     9342 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/change_subscription_status_claim_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    10169 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/changed_plan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/claim_response_subscription_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5510 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/confirm3ds_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3720 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8018 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4637 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response_card.py
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response_card_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11765 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response_dispute_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     8062 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/dispute_response_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7543 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/ewallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    10758 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/filing_recurring_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12222 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/filing_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/filing_request_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     4259 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/filing_request_subscription_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13315 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/filter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10996 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/flight.py
+-rw-rw-rw-   0 root         (0) root         (0)    17117 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/flights.py
+-rw-rw-rw-   0 root         (0) root         (0)    20816 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/installment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3692 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_creation_data_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4890 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_creation_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     7045 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7646 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8359 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_get_data_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     7069 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_get_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     6186 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     5102 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/invoice_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/item.py
+-rw-rw-rw-   0 root         (0) root         (0)     4089 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/limit_info_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/mobile_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/mobile_token_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3862 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/next_subscription_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5681 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/not_found_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     4765 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/o_auth_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    22171 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/oneclick_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11846 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     8326 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_confirm3ds_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_execute_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_gateway_creation_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_gateway_response_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7526 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_increment_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_methods_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     6143 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_patch_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    14704 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     9784 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_card.py
+-rw-rw-rw-   0 root         (0) root         (0)    10524 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_card_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_cryptocurrency_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    24043 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9885 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_e_wallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     8837 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_living_address.py
+-rw-rw-rw-   0 root         (0) root         (0)    11036 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)    24815 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_request_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7973 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12115 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_response_card_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     7192 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_response_cryptocurrency_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    13026 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_response_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    23247 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_response_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7466 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_update_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5410 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payment_update_transaction_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4577 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payments_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12413 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_creation_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4248 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13066 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_card.py
+-rw-rw-rw-   0 root         (0) root         (0)     7928 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_card_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_cryptocurrency_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    16987 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    10769 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_e_wallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     9023 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_living_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     6313 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     9324 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_request_payout_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12397 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    10792 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_response_card_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     7076 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_response_cryptocurrency_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     7034 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_response_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_response_e_wallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)    13951 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_response_payout_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4710 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5117 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payout_update_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/payouts_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/pix_account_details_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/pix_account_details_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4583 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/plan_data_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6809 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/plan_quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6534 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/plan_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6484 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/plan_update_request_plan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/plan_update_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     9077 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     8431 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_confirm3ds_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_creation_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17547 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9245 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6621 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_execute_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    15170 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_filter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_gateway_creation_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5024 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_gateway_response_recurring_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7623 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_increment_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_patch_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_plan_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13848 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_plan_request_plan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_plan_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4517 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_request_filing.py
+-rw-rw-rw-   0 root         (0) root         (0)    27321 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_request_recurring_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     9166 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3936 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_response_filing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5115 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_response_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)    31219 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_response_recurring_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7563 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6612 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurring_update_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/recurrings_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/redirect_url_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11182 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     8960 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6959 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_request_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     8267 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_request_e_wallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5521 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_request_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     3893 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_request_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5103 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_request_refund_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10175 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     7961 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_response_card_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     6319 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_response_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3766 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_response_e_wallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4705 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_response_payment_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_response_refund_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5117 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refund_update_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/refunds_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    10169 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/renamed_plan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11448 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     6065 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/reports_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/reports_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/reports_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4597 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/request_updated_transaction_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12878 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/response_plan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/response_updated_transaction_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/return_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    18412 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/scheduled_by_merchant_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19286 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/scheduled_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/shipping_address.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription.py
+-rw-rw-rw-   0 root         (0) root         (0)     4377 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    17289 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_filter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    23206 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_get_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3664 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_get_response_plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_pending_plan_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     9092 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_update_request_subscription_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4061 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/subscription_update_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4393 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/supported_payment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     9996 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/three_d_secure_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    16067 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/three_d_secure_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5094 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/transaction_methods_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/transaction_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5407 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/transaction_response_e_wallet_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     5105 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/transaction_response_merchant_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/transaction_update_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10169 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/updated_plan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    16550 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/updated_subscription_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/model/updated_subscription_recurring_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    14892 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32460 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7335 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    13856 2024-06-03 06:12:39.000000 cardpay-3.73.6/cardpay/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8129 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-06-03 06:12:56.000000 cardpay-3.73.6/cardpay.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-06-03 06:12:39.000000 cardpay-3.73.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2024-06-03 06:12:39.000000 cardpay-3.73.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-06-03 06:12:56.000000 cardpay-3.73.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-06-03 06:12:56.000000 cardpay-3.73.6/setup.py
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-06-03 06:12:56.000000 cardpay-3.73.6/PKG-INFO
```

### Comparing `cardpay-3.68.8/cardpay/api/auth_api.py` & `cardpay-3.73.6/cardpay/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/authentication_api.py` & `cardpay-3.73.6/cardpay/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/card_info_api.py` & `cardpay-3.73.6/cardpay/api/card_info_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/invoices_api.py` & `cardpay-3.73.6/cardpay/api/invoices_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/limits_api.py` & `cardpay-3.73.6/cardpay/api/limits_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/mobile_api.py` & `cardpay-3.73.6/cardpay/api/mobile_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/payments_api.py` & `cardpay-3.73.6/cardpay/api/payments_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/payouts_api.py` & `cardpay-3.73.6/cardpay/api/payouts_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/pix_account_details_api.py` & `cardpay-3.73.6/cardpay/api/pix_account_details_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/recurrings_api.py` & `cardpay-3.73.6/cardpay/api/recurrings_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/refunds_api.py` & `cardpay-3.73.6/cardpay/api/refunds_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api/reports_api_controller_api.py` & `cardpay-3.73.6/cardpay/api/reports_api_controller_api.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/api_error.py` & `cardpay-3.73.6/cardpay/model/api_error.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/api_tokens.py` & `cardpay-3.73.6/cardpay/model/api_tokens.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/auth_data_request.py` & `cardpay-3.73.6/cardpay/model/auth_data_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/authentication_create_response.py` & `cardpay-3.73.6/cardpay/model/authentication_create_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/authentication_customer.py` & `cardpay-3.73.6/cardpay/model/authentication_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/authentication_data.py` & `cardpay-3.73.6/cardpay/model/authentication_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/authentication_data_request.py` & `cardpay-3.73.6/cardpay/model/authentication_data_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/authentication_data_response.py` & `cardpay-3.73.6/cardpay/model/authentication_data_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/authentication_error.py` & `cardpay-3.73.6/cardpay/model/authentication_error.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/bad_request_error.py` & `cardpay-3.73.6/cardpay/model/bad_request_error.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/bank_card_payout_data.py` & `cardpay-3.73.6/cardpay/model/bank_card_payout_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/billing_address.py` & `cardpay-3.73.6/cardpay/model/billing_address.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/browser_info.py` & `cardpay-3.73.6/cardpay/model/browser_info.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/card_info_request.py` & `cardpay-3.73.6/cardpay/model/card_info_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/card_info_response.py` & `cardpay-3.73.6/cardpay/model/card_info_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/change_subscription_status_claim_response.py` & `cardpay-3.73.6/cardpay/model/change_subscription_status_claim_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/changed_plan_data.py` & `cardpay-3.73.6/cardpay/model/changed_plan_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/claim_response_subscription_data.py` & `cardpay-3.73.6/cardpay/model/claim_response_subscription_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/confirm3ds_request.py` & `cardpay-3.73.6/cardpay/model/confirm3ds_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/device.py` & `cardpay-3.73.6/cardpay/model/device.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_list.py` & `cardpay-3.73.6/cardpay/model/dispute_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response.py` & `cardpay-3.73.6/cardpay/model/dispute_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response_card.py` & `cardpay-3.73.6/cardpay/model/dispute_response_card.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response_card_account.py` & `cardpay-3.73.6/cardpay/model/dispute_response_card_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response_customer.py` & `cardpay-3.73.6/cardpay/model/dispute_response_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response_dispute_data.py` & `cardpay-3.73.6/cardpay/model/dispute_response_dispute_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response_merchant_order.py` & `cardpay-3.73.6/cardpay/model/dispute_response_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/dispute_response_payment_data.py` & `cardpay-3.73.6/cardpay/model/dispute_response_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/ewallet_account.py` & `cardpay-3.73.6/cardpay/model/ewallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/filing_recurring_data.py` & `cardpay-3.73.6/cardpay/model/filing_recurring_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/filing_request.py` & `cardpay-3.73.6/cardpay/model/filing_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/filing_request_merchant_order.py` & `cardpay-3.73.6/cardpay/model/filing_request_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/filing_request_subscription_data.py` & `cardpay-3.73.6/cardpay/model/filing_request_subscription_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/filter_parameters.py` & `cardpay-3.73.6/cardpay/model/filter_parameters.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/flight.py` & `cardpay-3.73.6/cardpay/model/flight.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/flights.py` & `cardpay-3.73.6/cardpay/model/flights.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/installment_data.py` & `cardpay-3.73.6/cardpay/model/installment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_creation_data_response.py` & `cardpay-3.73.6/cardpay/model/invoice_creation_data_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_creation_response.py` & `cardpay-3.73.6/cardpay/model/invoice_creation_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_customer.py` & `cardpay-3.73.6/cardpay/model/invoice_merchant_order.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,124 +12,103 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+from cardpay.model.invoice_item import InvoiceItem  # noqa: F401,E501
 
-class InvoiceCustomer(object):
+
+class InvoiceMerchantOrder(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"email": "str", "id": "str", "phone": "str"}
+    swagger_types = {"id": "str", "items": "list[InvoiceItem]"}
 
-    attribute_map = {"email": "email", "id": "id", "phone": "phone"}
+    attribute_map = {"id": "id", "items": "items"}
 
-    def __init__(self, email=None, id=None, phone=None):  # noqa: E501
-        """InvoiceCustomer - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, id=None, items=None):  # noqa: E501
+        """InvoiceMerchantOrder - a model defined in Swagger"""  # noqa: E501
 
-        self._email = None
         self._id = None
-        self._phone = None
+        self._items = None
         self.discriminator = None
 
-        if email is not None:
-            self.email = email
         self.id = id
-        if phone is not None:
-            self.phone = phone
-
-    @property
-    def email(self):
-        """Gets the email of this InvoiceCustomer.  # noqa: E501
-
-        Email address of the customer  # noqa: E501
-
-        :return: The email of this InvoiceCustomer.  # noqa: E501
-        :rtype: str
-        """
-        return self._email
-
-    @email.setter
-    def email(self, email):
-        """Sets the email of this InvoiceCustomer.
-
-        Email address of the customer  # noqa: E501
-
-        :param email: The email of this InvoiceCustomer.  # noqa: E501
-        :type: str
-        """
-
-        self._email = email
+        self.items = items
 
     @property
     def id(self):
-        """Gets the id of this InvoiceCustomer.  # noqa: E501
+        """Gets the id of this InvoiceMerchantOrder.  # noqa: E501
 
-        Customer's ID in Merchant's system  # noqa: E501
+        Order ID used by the merchant’s shopping cart  # noqa: E501
 
-        :return: The id of this InvoiceCustomer.  # noqa: E501
+        :return: The id of this InvoiceMerchantOrder.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this InvoiceCustomer.
+        """Sets the id of this InvoiceMerchantOrder.
 
-        Customer's ID in Merchant's system  # noqa: E501
+        Order ID used by the merchant’s shopping cart  # noqa: E501
 
-        :param id: The id of this InvoiceCustomer.  # noqa: E501
+        :param id: The id of this InvoiceMerchantOrder.  # noqa: E501
         :type: str
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if id is not None and len(id) > 256:
+        if id is not None and len(id) > 50:
             raise ValueError(
-                "Invalid value for `id`, length must be less than or equal to `256`"
+                "Invalid value for `id`, length must be less than or equal to `50`"
             )  # noqa: E501
-        if id is not None and len(id) < 0:
+        if id is not None and len(id) < 1:
             raise ValueError(
-                "Invalid value for `id`, length must be greater than or equal to `0`"
+                "Invalid value for `id`, length must be greater than or equal to `1`"
             )  # noqa: E501
 
         self._id = id
 
     @property
-    def phone(self):
-        """Gets the phone of this InvoiceCustomer.  # noqa: E501
+    def items(self):
+        """Gets the items of this InvoiceMerchantOrder.  # noqa: E501
 
-        Customer phone number  # noqa: E501
+        Array of items (in the shopping cart)  # noqa: E501
 
-        :return: The phone of this InvoiceCustomer.  # noqa: E501
-        :rtype: str
+        :return: The items of this InvoiceMerchantOrder.  # noqa: E501
+        :rtype: list[InvoiceItem]
         """
-        return self._phone
+        return self._items
 
-    @phone.setter
-    def phone(self, phone):
-        """Sets the phone of this InvoiceCustomer.
+    @items.setter
+    def items(self, items):
+        """Sets the items of this InvoiceMerchantOrder.
 
-        Customer phone number  # noqa: E501
+        Array of items (in the shopping cart)  # noqa: E501
 
-        :param phone: The phone of this InvoiceCustomer.  # noqa: E501
-        :type: str
+        :param items: The items of this InvoiceMerchantOrder.  # noqa: E501
+        :type: list[InvoiceItem]
         """
+        if items is None:
+            raise ValueError(
+                "Invalid value for `items`, must not be `None`"
+            )  # noqa: E501
 
-        self._phone = phone
+        self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -147,15 +126,15 @@
                         else item,
                         value.items(),
                     )
                 )
             else:
                 if value is not None:
                     result[attr] = value
-        if issubclass(InvoiceCustomer, dict):
+        if issubclass(InvoiceMerchantOrder, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -163,15 +142,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InvoiceCustomer):
+        if not isinstance(other, InvoiceMerchantOrder):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cardpay-3.68.8/cardpay/model/invoice_data.py` & `cardpay-3.73.6/cardpay/model/invoice_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_get_data_response.py` & `cardpay-3.73.6/cardpay/model/invoice_get_data_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_get_response.py` & `cardpay-3.73.6/cardpay/model/invoice_get_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_item.py` & `cardpay-3.73.6/cardpay/model/invoice_item.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/invoice_merchant_order.py` & `cardpay-3.73.6/cardpay/model/subscription_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,103 +12,93 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cardpay.model.invoice_item import InvoiceItem  # noqa: F401,E501
+from cardpay.model.subscription_get_response import (
+    SubscriptionGetResponse,
+)  # noqa: F401,E501
 
 
-class InvoiceMerchantOrder(object):
+class SubscriptionList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"id": "str", "items": "list[InvoiceItem]"}
+    swagger_types = {"data": "list[SubscriptionGetResponse]", "has_more": "bool"}
 
-    attribute_map = {"id": "id", "items": "items"}
+    attribute_map = {"data": "data", "has_more": "has_more"}
 
-    def __init__(self, id=None, items=None):  # noqa: E501
-        """InvoiceMerchantOrder - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, data=None, has_more=None):  # noqa: E501
+        """SubscriptionList - a model defined in Swagger"""  # noqa: E501
 
-        self._id = None
-        self._items = None
+        self._data = None
+        self._has_more = None
         self.discriminator = None
 
-        self.id = id
-        self.items = items
+        if data is not None:
+            self.data = data
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def id(self):
-        """Gets the id of this InvoiceMerchantOrder.  # noqa: E501
+    def data(self):
+        """Gets the data of this SubscriptionList.  # noqa: E501
 
-        Order ID used by the merchant’s shopping cart  # noqa: E501
+        List of found objects  # noqa: E501
 
-        :return: The id of this InvoiceMerchantOrder.  # noqa: E501
-        :rtype: str
+        :return: The data of this SubscriptionList.  # noqa: E501
+        :rtype: list[SubscriptionGetResponse]
         """
-        return self._id
+        return self._data
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this InvoiceMerchantOrder.
+    @data.setter
+    def data(self, data):
+        """Sets the data of this SubscriptionList.
 
-        Order ID used by the merchant’s shopping cart  # noqa: E501
+        List of found objects  # noqa: E501
 
-        :param id: The id of this InvoiceMerchantOrder.  # noqa: E501
-        :type: str
+        :param data: The data of this SubscriptionList.  # noqa: E501
+        :type: list[SubscriptionGetResponse]
         """
-        if id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if id is not None and len(id) > 50:
-            raise ValueError(
-                "Invalid value for `id`, length must be less than or equal to `50`"
-            )  # noqa: E501
-        if id is not None and len(id) < 1:
-            raise ValueError(
-                "Invalid value for `id`, length must be greater than or equal to `1`"
-            )  # noqa: E501
 
-        self._id = id
+        self._data = data
 
     @property
-    def items(self):
-        """Gets the items of this InvoiceMerchantOrder.  # noqa: E501
+    def has_more(self):
+        """Gets the has_more of this SubscriptionList.  # noqa: E501
 
-        Array of items (in the shopping cart)  # noqa: E501
+        Indicates if there are more elements for this period than were returned  # noqa: E501
 
-        :return: The items of this InvoiceMerchantOrder.  # noqa: E501
-        :rtype: list[InvoiceItem]
+        :return: The has_more of this SubscriptionList.  # noqa: E501
+        :rtype: bool
         """
-        return self._items
+        return self._has_more
 
-    @items.setter
-    def items(self, items):
-        """Sets the items of this InvoiceMerchantOrder.
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this SubscriptionList.
 
-        Array of items (in the shopping cart)  # noqa: E501
+        Indicates if there are more elements for this period than were returned  # noqa: E501
 
-        :param items: The items of this InvoiceMerchantOrder.  # noqa: E501
-        :type: list[InvoiceItem]
+        :param has_more: The has_more of this SubscriptionList.  # noqa: E501
+        :type: bool
         """
-        if items is None:
-            raise ValueError(
-                "Invalid value for `items`, must not be `None`"
-            )  # noqa: E501
 
-        self._items = items
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -126,15 +116,15 @@
                         else item,
                         value.items(),
                     )
                 )
             else:
                 if value is not None:
                     result[attr] = value
-        if issubclass(InvoiceMerchantOrder, dict):
+        if issubclass(SubscriptionList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -142,15 +132,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InvoiceMerchantOrder):
+        if not isinstance(other, SubscriptionList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cardpay-3.68.8/cardpay/model/invoice_request.py` & `cardpay-3.73.6/cardpay/model/invoice_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/item.py` & `cardpay-3.73.6/cardpay/model/item.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/limit_info_response.py` & `cardpay-3.73.6/cardpay/model/limit_info_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/mobile_token_request.py` & `cardpay-3.73.6/cardpay/model/mobile_token_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/mobile_token_response.py` & `cardpay-3.73.6/cardpay/model/mobile_token_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/next_subscription_payment.py` & `cardpay-3.73.6/cardpay/model/next_subscription_payment.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/not_found_error.py` & `cardpay-3.73.6/cardpay/model/not_found_error.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/o_auth_error.py` & `cardpay-3.73.6/cardpay/model/o_auth_error.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/oneclick_data.py` & `cardpay-3.73.6/cardpay/model/oneclick_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_callback.py` & `cardpay-3.73.6/cardpay/model/payment_callback.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_confirm3ds_request.py` & `cardpay-3.73.6/cardpay/model/payment_confirm3ds_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_execute_request.py` & `cardpay-3.73.6/cardpay/model/payment_execute_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_gateway_creation_response.py` & `cardpay-3.73.6/cardpay/model/payment_gateway_creation_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_gateway_response_payment_data.py` & `cardpay-3.73.6/cardpay/model/payment_gateway_response_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_increment_request.py` & `cardpay-3.73.6/cardpay/model/payment_increment_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_methods_response.py` & `cardpay-3.73.6/cardpay/model/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_patch_request.py` & `cardpay-3.73.6/cardpay/model/payment_patch_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request.py` & `cardpay-3.73.6/cardpay/model/payment_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_card.py` & `cardpay-3.73.6/cardpay/model/payment_request_card.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_card_account.py` & `cardpay-3.73.6/cardpay/model/payment_request_card_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_cryptocurrency_account.py` & `cardpay-3.73.6/cardpay/model/payment_request_cryptocurrency_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_customer.py` & `cardpay-3.73.6/cardpay/model/payment_request_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_e_wallet_account.py` & `cardpay-3.73.6/cardpay/model/payment_request_e_wallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_living_address.py` & `cardpay-3.73.6/cardpay/model/payment_request_living_address.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_merchant_order.py` & `cardpay-3.73.6/cardpay/model/payment_request_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_request_payment_data.py` & `cardpay-3.73.6/cardpay/model/payment_request_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_response.py` & `cardpay-3.73.6/cardpay/model/payment_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_response_card_account.py` & `cardpay-3.73.6/cardpay/model/payment_response_card_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_response_cryptocurrency_account.py` & `cardpay-3.73.6/cardpay/model/payment_response_cryptocurrency_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_response_customer.py` & `cardpay-3.73.6/cardpay/model/payment_response_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_response_payment_data.py` & `cardpay-3.73.6/cardpay/model/payment_response_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_update_request.py` & `cardpay-3.73.6/cardpay/model/payment_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_update_response.py` & `cardpay-3.73.6/cardpay/model/payment_update_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payment_update_transaction_data.py` & `cardpay-3.73.6/cardpay/model/payment_update_transaction_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payments_list.py` & `cardpay-3.73.6/cardpay/model/payments_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_callback.py` & `cardpay-3.73.6/cardpay/model/payout_callback.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_creation_response.py` & `cardpay-3.73.6/cardpay/model/payout_creation_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_payment_data.py` & `cardpay-3.73.6/cardpay/model/payout_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request.py` & `cardpay-3.73.6/cardpay/model/payout_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_card.py` & `cardpay-3.73.6/cardpay/model/payout_request_card.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_card_account.py` & `cardpay-3.73.6/cardpay/model/payout_request_card_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_cryptocurrency_account.py` & `cardpay-3.73.6/cardpay/model/payout_request_cryptocurrency_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_customer.py` & `cardpay-3.73.6/cardpay/model/payout_request_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_e_wallet_account.py` & `cardpay-3.73.6/cardpay/model/payout_request_e_wallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_living_address.py` & `cardpay-3.73.6/cardpay/model/payout_request_living_address.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_merchant_order.py` & `cardpay-3.73.6/cardpay/model/payout_request_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_request_payout_data.py` & `cardpay-3.73.6/cardpay/model/payout_request_payout_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_response.py` & `cardpay-3.73.6/cardpay/model/payout_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_response_card_account.py` & `cardpay-3.73.6/cardpay/model/payout_response_card_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_response_cryptocurrency_account.py` & `cardpay-3.73.6/cardpay/model/payout_response_cryptocurrency_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_response_customer.py` & `cardpay-3.73.6/cardpay/model/payout_response_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_response_e_wallet_account.py` & `cardpay-3.73.6/cardpay/model/payout_response_e_wallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_response_payout_data.py` & `cardpay-3.73.6/cardpay/model/payout_response_payout_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/plan.py` & `cardpay-3.73.6/cardpay/model/plan.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_update_request.py` & `cardpay-3.73.6/cardpay/model/payout_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payout_update_response.py` & `cardpay-3.73.6/cardpay/model/payout_update_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/payouts_list.py` & `cardpay-3.73.6/cardpay/model/payouts_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/pix_account_details_request.py` & `cardpay-3.73.6/cardpay/model/pix_account_details_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/pix_account_details_response.py` & `cardpay-3.73.6/cardpay/model/pix_account_details_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/plan_data_list.py` & `cardpay-3.73.6/cardpay/model/plan_data_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/plan_quantity.py` & `cardpay-3.73.6/cardpay/model/plan_quantity.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/plan_update_request.py` & `cardpay-3.73.6/cardpay/model/plan_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/plan_update_request_plan_data.py` & `cardpay-3.73.6/cardpay/model/plan_update_request_plan_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/plan_update_response.py` & `cardpay-3.73.6/cardpay/model/plan_update_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_callback.py` & `cardpay-3.73.6/cardpay/model/recurring_callback.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_confirm3ds_request.py` & `cardpay-3.73.6/cardpay/model/recurring_confirm3ds_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_creation_request.py` & `cardpay-3.73.6/cardpay/model/recurring_creation_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_customer.py` & `cardpay-3.73.6/cardpay/model/recurring_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_data.py` & `cardpay-3.73.6/cardpay/model/recurring_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_execute_request.py` & `cardpay-3.73.6/cardpay/model/recurring_execute_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_filter_parameters.py` & `cardpay-3.73.6/cardpay/model/recurring_filter_parameters.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_gateway_creation_response.py` & `cardpay-3.73.6/cardpay/model/recurring_gateway_creation_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_gateway_response_recurring_data.py` & `cardpay-3.73.6/cardpay/model/recurring_gateway_response_recurring_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_increment_request.py` & `cardpay-3.73.6/cardpay/model/recurring_increment_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_patch_request.py` & `cardpay-3.73.6/cardpay/model/recurring_patch_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_plan_request.py` & `cardpay-3.73.6/cardpay/model/recurring_plan_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_plan_request_plan_data.py` & `cardpay-3.73.6/cardpay/model/recurring_plan_request_plan_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_plan_response.py` & `cardpay-3.73.6/cardpay/model/recurring_plan_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_request_filing.py` & `cardpay-3.73.6/cardpay/model/recurring_request_filing.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_request_recurring_data.py` & `cardpay-3.73.6/cardpay/model/recurring_request_recurring_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_response.py` & `cardpay-3.73.6/cardpay/model/recurring_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_response_filing.py` & `cardpay-3.73.6/cardpay/model/recurring_response_filing.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_response_merchant_order.py` & `cardpay-3.73.6/cardpay/model/recurring_response_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_response_recurring_data.py` & `cardpay-3.73.6/cardpay/model/recurring_response_recurring_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_update_request.py` & `cardpay-3.73.6/cardpay/model/recurring_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurring_update_response.py` & `cardpay-3.73.6/cardpay/model/recurring_update_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/recurrings_list.py` & `cardpay-3.73.6/cardpay/model/recurrings_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/redirect_url_response.py` & `cardpay-3.73.6/cardpay/model/redirect_url_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_callback.py` & `cardpay-3.73.6/cardpay/model/refund_callback.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_request.py` & `cardpay-3.73.6/cardpay/model/refund_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_request_customer.py` & `cardpay-3.73.6/cardpay/model/refund_request_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_request_e_wallet_account.py` & `cardpay-3.73.6/cardpay/model/refund_request_e_wallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_request_merchant_order.py` & `cardpay-3.73.6/cardpay/model/refund_request_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_request_payment_data.py` & `cardpay-3.73.6/cardpay/model/refund_request_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_request_refund_data.py` & `cardpay-3.73.6/cardpay/model/refund_request_refund_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_response.py` & `cardpay-3.73.6/cardpay/model/refund_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_response_card_account.py` & `cardpay-3.73.6/cardpay/model/refund_response_card_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_response_customer.py` & `cardpay-3.73.6/cardpay/model/refund_response_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_response_e_wallet_account.py` & `cardpay-3.73.6/cardpay/model/refund_response_e_wallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_response_payment_data.py` & `cardpay-3.73.6/cardpay/model/refund_response_payment_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_response_refund_data.py` & `cardpay-3.73.6/cardpay/model/refund_response_refund_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_update_request.py` & `cardpay-3.73.6/cardpay/model/refund_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refund_update_response.py` & `cardpay-3.73.6/cardpay/model/refund_update_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/refunds_list.py` & `cardpay-3.73.6/cardpay/model/refunds_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/renamed_plan_data.py` & `cardpay-3.73.6/cardpay/model/renamed_plan_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/report.py` & `cardpay-3.73.6/cardpay/model/report.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/reports_data.py` & `cardpay-3.73.6/cardpay/model/reports_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/reports_request.py` & `cardpay-3.73.6/cardpay/model/reports_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/reports_response.py` & `cardpay-3.73.6/cardpay/model/reports_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/request.py` & `cardpay-3.73.6/cardpay/model/request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/request_updated_transaction_data.py` & `cardpay-3.73.6/cardpay/model/request_updated_transaction_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/response_plan_data.py` & `cardpay-3.73.6/cardpay/model/response_plan_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/response_updated_transaction_data.py` & `cardpay-3.73.6/cardpay/model/response_updated_transaction_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/return_urls.py` & `cardpay-3.73.6/cardpay/model/return_urls.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/scheduled_by_merchant_data.py` & `cardpay-3.73.6/cardpay/model/scheduled_by_merchant_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/scheduled_data.py` & `cardpay-3.73.6/cardpay/model/scheduled_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/shipping_address.py` & `cardpay-3.73.6/cardpay/model/shipping_address.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription.py` & `cardpay-3.73.6/cardpay/model/subscription.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_customer.py` & `cardpay-3.73.6/cardpay/model/subscription_customer.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_filter_parameters.py` & `cardpay-3.73.6/cardpay/model/subscription_filter_parameters.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_get_response.py` & `cardpay-3.73.6/cardpay/model/subscription_get_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_get_response_plan.py` & `cardpay-3.73.6/cardpay/model/subscription_get_response_plan.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_list.py` & `cardpay-3.73.6/cardpay/model/subscription_pending_plan_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,93 +12,89 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cardpay.model.subscription_get_response import (
-    SubscriptionGetResponse,
-)  # noqa: F401,E501
 
-
-class SubscriptionList(object):
+class SubscriptionPendingPlanUpdate(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"data": "list[SubscriptionGetResponse]", "has_more": "bool"}
+    swagger_types = {"_date": "str", "id": "str"}
 
-    attribute_map = {"data": "data", "has_more": "has_more"}
+    attribute_map = {"_date": "date", "id": "id"}
 
-    def __init__(self, data=None, has_more=None):  # noqa: E501
-        """SubscriptionList - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, _date=None, id=None):  # noqa: E501
+        """SubscriptionPendingPlanUpdate - a model defined in Swagger"""  # noqa: E501
 
-        self._data = None
-        self._has_more = None
+        self.__date = None
+        self._id = None
         self.discriminator = None
 
-        if data is not None:
-            self.data = data
-        if has_more is not None:
-            self.has_more = has_more
+        if _date is not None:
+            self._date = _date
+        if id is not None:
+            self.id = id
 
     @property
-    def data(self):
-        """Gets the data of this SubscriptionList.  # noqa: E501
+    def _date(self):
+        """Gets the _date of this SubscriptionPendingPlanUpdate.  # noqa: E501
 
-        List of found objects  # noqa: E501
+        Plan change date  # noqa: E501
 
-        :return: The data of this SubscriptionList.  # noqa: E501
-        :rtype: list[SubscriptionGetResponse]
+        :return: The _date of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._data
+        return self.__date
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this SubscriptionList.
+    @_date.setter
+    def _date(self, _date):
+        """Sets the _date of this SubscriptionPendingPlanUpdate.
 
-        List of found objects  # noqa: E501
+        Plan change date  # noqa: E501
 
-        :param data: The data of this SubscriptionList.  # noqa: E501
-        :type: list[SubscriptionGetResponse]
+        :param _date: The _date of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :type: str
         """
 
-        self._data = data
+        self.__date = _date
 
     @property
-    def has_more(self):
-        """Gets the has_more of this SubscriptionList.  # noqa: E501
+    def id(self):
+        """Gets the id of this SubscriptionPendingPlanUpdate.  # noqa: E501
 
-        Indicates if there are more elements for this period than were returned  # noqa: E501
+        Subscription plan id  # noqa: E501
 
-        :return: The has_more of this SubscriptionList.  # noqa: E501
-        :rtype: bool
+        :return: The id of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._has_more
+        return self._id
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this SubscriptionList.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this SubscriptionPendingPlanUpdate.
 
-        Indicates if there are more elements for this period than were returned  # noqa: E501
+        Subscription plan id  # noqa: E501
 
-        :param has_more: The has_more of this SubscriptionList.  # noqa: E501
-        :type: bool
+        :param id: The id of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :type: str
         """
 
-        self._has_more = has_more
+        self._id = id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -116,15 +112,15 @@
                         else item,
                         value.items(),
                     )
                 )
             else:
                 if value is not None:
                     result[attr] = value
-        if issubclass(SubscriptionList, dict):
+        if issubclass(SubscriptionPendingPlanUpdate, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,15 +128,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubscriptionList):
+        if not isinstance(other, SubscriptionPendingPlanUpdate):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cardpay-3.68.8/cardpay/model/subscription_pending_plan_update.py` & `cardpay-3.73.6/cardpay/model/supported_payment_method.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,88 +13,88 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class SubscriptionPendingPlanUpdate(object):
+class SupportedPaymentMethod(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"_date": "str", "id": "str"}
+    swagger_types = {"logo": "str", "name": "str"}
 
-    attribute_map = {"_date": "date", "id": "id"}
+    attribute_map = {"logo": "logo", "name": "name"}
 
-    def __init__(self, _date=None, id=None):  # noqa: E501
-        """SubscriptionPendingPlanUpdate - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, logo=None, name=None):  # noqa: E501
+        """SupportedPaymentMethod - a model defined in Swagger"""  # noqa: E501
 
-        self.__date = None
-        self._id = None
+        self._logo = None
+        self._name = None
         self.discriminator = None
 
-        if _date is not None:
-            self._date = _date
-        if id is not None:
-            self.id = id
+        if logo is not None:
+            self.logo = logo
+        if name is not None:
+            self.name = name
 
     @property
-    def _date(self):
-        """Gets the _date of this SubscriptionPendingPlanUpdate.  # noqa: E501
+    def logo(self):
+        """Gets the logo of this SupportedPaymentMethod.  # noqa: E501
 
-        Plan change date  # noqa: E501
+        Url to Payment Method logo  # noqa: E501
 
-        :return: The _date of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :return: The logo of this SupportedPaymentMethod.  # noqa: E501
         :rtype: str
         """
-        return self.__date
+        return self._logo
 
-    @_date.setter
-    def _date(self, _date):
-        """Sets the _date of this SubscriptionPendingPlanUpdate.
+    @logo.setter
+    def logo(self, logo):
+        """Sets the logo of this SupportedPaymentMethod.
 
-        Plan change date  # noqa: E501
+        Url to Payment Method logo  # noqa: E501
 
-        :param _date: The _date of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :param logo: The logo of this SupportedPaymentMethod.  # noqa: E501
         :type: str
         """
 
-        self.__date = _date
+        self._logo = logo
 
     @property
-    def id(self):
-        """Gets the id of this SubscriptionPendingPlanUpdate.  # noqa: E501
+    def name(self):
+        """Gets the name of this SupportedPaymentMethod.  # noqa: E501
 
-        Subscription plan id  # noqa: E501
+        Name of Payment Method  # noqa: E501
 
-        :return: The id of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :return: The name of this SupportedPaymentMethod.  # noqa: E501
         :rtype: str
         """
-        return self._id
+        return self._name
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this SubscriptionPendingPlanUpdate.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this SupportedPaymentMethod.
 
-        Subscription plan id  # noqa: E501
+        Name of Payment Method  # noqa: E501
 
-        :param id: The id of this SubscriptionPendingPlanUpdate.  # noqa: E501
+        :param name: The name of this SupportedPaymentMethod.  # noqa: E501
         :type: str
         """
 
-        self._id = id
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -112,15 +112,15 @@
                         else item,
                         value.items(),
                     )
                 )
             else:
                 if value is not None:
                     result[attr] = value
-        if issubclass(SubscriptionPendingPlanUpdate, dict):
+        if issubclass(SupportedPaymentMethod, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -128,15 +128,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubscriptionPendingPlanUpdate):
+        if not isinstance(other, SupportedPaymentMethod):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cardpay-3.68.8/cardpay/model/subscription_update_request.py` & `cardpay-3.73.6/cardpay/model/subscription_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_update_request_subscription_data.py` & `cardpay-3.73.6/cardpay/model/subscription_update_request_subscription_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/subscription_update_response.py` & `cardpay-3.73.6/cardpay/model/subscription_update_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/supported_payment_method.py` & `cardpay-3.73.6/cardpay/model/updated_subscription_recurring_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,88 +13,88 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class SupportedPaymentMethod(object):
+class UpdatedSubscriptionRecurringData(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {"logo": "str", "name": "str"}
+    swagger_types = {"id": "str", "separate_auth": "bool"}
 
-    attribute_map = {"logo": "logo", "name": "name"}
+    attribute_map = {"id": "id", "separate_auth": "separate_auth"}
 
-    def __init__(self, logo=None, name=None):  # noqa: E501
-        """SupportedPaymentMethod - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, id=None, separate_auth=None):  # noqa: E501
+        """UpdatedSubscriptionRecurringData - a model defined in Swagger"""  # noqa: E501
 
-        self._logo = None
-        self._name = None
+        self._id = None
+        self._separate_auth = None
         self.discriminator = None
 
-        if logo is not None:
-            self.logo = logo
-        if name is not None:
-            self.name = name
+        if id is not None:
+            self.id = id
+        if separate_auth is not None:
+            self.separate_auth = separate_auth
 
     @property
-    def logo(self):
-        """Gets the logo of this SupportedPaymentMethod.  # noqa: E501
+    def id(self):
+        """Gets the id of this UpdatedSubscriptionRecurringData.  # noqa: E501
 
-        Url to Payment Method logo  # noqa: E501
+        ID of transaction initiated by repayment request.  # noqa: E501
 
-        :return: The logo of this SupportedPaymentMethod.  # noqa: E501
+        :return: The id of this UpdatedSubscriptionRecurringData.  # noqa: E501
         :rtype: str
         """
-        return self._logo
+        return self._id
 
-    @logo.setter
-    def logo(self, logo):
-        """Sets the logo of this SupportedPaymentMethod.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this UpdatedSubscriptionRecurringData.
 
-        Url to Payment Method logo  # noqa: E501
+        ID of transaction initiated by repayment request.  # noqa: E501
 
-        :param logo: The logo of this SupportedPaymentMethod.  # noqa: E501
+        :param id: The id of this UpdatedSubscriptionRecurringData.  # noqa: E501
         :type: str
         """
 
-        self._logo = logo
+        self._id = id
 
     @property
-    def name(self):
-        """Gets the name of this SupportedPaymentMethod.  # noqa: E501
+    def separate_auth(self):
+        """Gets the separate_auth of this UpdatedSubscriptionRecurringData.  # noqa: E501
 
-        Name of Payment Method  # noqa: E501
+        Means that authentication can be carried separately from the payment. Possible values: true -  authentication can be carried separately, false -  authentication can not be carried separately  # noqa: E501
 
-        :return: The name of this SupportedPaymentMethod.  # noqa: E501
-        :rtype: str
+        :return: The separate_auth of this UpdatedSubscriptionRecurringData.  # noqa: E501
+        :rtype: bool
         """
-        return self._name
+        return self._separate_auth
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this SupportedPaymentMethod.
+    @separate_auth.setter
+    def separate_auth(self, separate_auth):
+        """Sets the separate_auth of this UpdatedSubscriptionRecurringData.
 
-        Name of Payment Method  # noqa: E501
+        Means that authentication can be carried separately from the payment. Possible values: true -  authentication can be carried separately, false -  authentication can not be carried separately  # noqa: E501
 
-        :param name: The name of this SupportedPaymentMethod.  # noqa: E501
-        :type: str
+        :param separate_auth: The separate_auth of this UpdatedSubscriptionRecurringData.  # noqa: E501
+        :type: bool
         """
 
-        self._name = name
+        self._separate_auth = separate_auth
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -112,15 +112,15 @@
                         else item,
                         value.items(),
                     )
                 )
             else:
                 if value is not None:
                     result[attr] = value
-        if issubclass(SupportedPaymentMethod, dict):
+        if issubclass(UpdatedSubscriptionRecurringData, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -128,15 +128,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SupportedPaymentMethod):
+        if not isinstance(other, UpdatedSubscriptionRecurringData):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cardpay-3.68.8/cardpay/model/three_d_secure_data.py` & `cardpay-3.73.6/cardpay/model/three_d_secure_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/three_d_secure_response.py` & `cardpay-3.73.6/cardpay/model/three_d_secure_response.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/transaction_methods_list.py` & `cardpay-3.73.6/cardpay/model/transaction_methods_list.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/transaction_request.py` & `cardpay-3.73.6/cardpay/model/transaction_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/transaction_response_e_wallet_account.py` & `cardpay-3.73.6/cardpay/model/transaction_response_e_wallet_account.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/transaction_response_merchant_order.py` & `cardpay-3.73.6/cardpay/model/transaction_response_merchant_order.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/transaction_update_request.py` & `cardpay-3.73.6/cardpay/model/transaction_update_request.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/updated_plan_data.py` & `cardpay-3.73.6/cardpay/model/updated_plan_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/model/updated_subscription_data.py` & `cardpay-3.73.6/cardpay/model/updated_subscription_data.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/__init__.py` & `cardpay-3.73.6/cardpay/__init__.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay/api_client.py` & `cardpay-3.73.6/cardpay/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         self._pool = None
         self.rest_client = ProxyRestClient.create(configuration)
         self.default_headers = {}
         self.tokens = None
         self.cookie = None
 
         # Set default User-Agent.
-        self.user_agent = "CardpaySdk/3.68.8/Python"
+        self.user_agent = "CardpaySdk/3.73.6/Python"
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
 
     def calc_signature(self, message):
```

### Comparing `cardpay-3.68.8/cardpay/configuration.py` & `cardpay-3.73.6/cardpay/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,11 +209,11 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 3.0\n"
-            "SDK Package Version: 3.68.8".format(
+            "SDK Package Version: 3.73.6".format(
                 env=sys.platform, pyversion=sys.version
             )
         )
```

### Comparing `cardpay-3.68.8/cardpay/rest.py` & `cardpay-3.73.6/cardpay/rest.py`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/cardpay.egg-info/PKG-INFO` & `cardpay-3.73.6/cardpay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardpay
-Version: 3.68.8
+Version: 3.73.6
 Summary: Unlimit APIv3 Python SDK
 Home-page: https://github.com/cardpay/python-sdk-v3.git
 Author-email: 
 License: MIT
 Project-URL: Source Code, https://github.com/cardpay/python-sdk-v3
 Project-URL: Documentation, https://integration.unlimit.com/
 Description: # Unlimit APIv3 Python SDK
@@ -27,15 +27,15 @@
         
         ```sh
         pip install git+https://github.com/cardpay/python-sdk-v3.git --upgrade
         ```
         or
         
         ```sh
-        pip install 'cardpay>=3.68.8' --upgrade
+        pip install 'cardpay>=3.73.6' --upgrade
         ```
         
         Then import the package:
         ```python
         from cardpay import *
         ```
```

### Comparing `cardpay-3.68.8/cardpay.egg-info/SOURCES.txt` & `cardpay-3.73.6/cardpay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/LICENSE` & `cardpay-3.73.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cardpay-3.68.8/README.md` & `cardpay-3.73.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ```sh
 pip install git+https://github.com/cardpay/python-sdk-v3.git --upgrade
 ```
 or
 
 ```sh
-pip install 'cardpay>=3.68.8' --upgrade
+pip install 'cardpay>=3.73.6' --upgrade
 ```
 
 Then import the package:
 ```python
 from cardpay import *
 ```
```

### Comparing `cardpay-3.68.8/setup.py` & `cardpay-3.73.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.chdir(here)
 
 with open(os.path.join(here, "README.md"), "r", encoding="utf-8") as fp:
     long_description = fp.read()
 
 setup(
     name="cardpay",
-    version="3.68.8",
+    version="3.73.6",
     description="Unlimit APIv3 Python SDK",
     author_email="",
     url="https://github.com/cardpay/python-sdk-v3.git",
     license="MIT",
     keywords=["cardpay", "APIv3", "CardPay REST API"],
     install_requires=[
         "certifi>=2019.11.28",
```

### Comparing `cardpay-3.68.8/PKG-INFO` & `cardpay-3.73.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardpay
-Version: 3.68.8
+Version: 3.73.6
 Summary: Unlimit APIv3 Python SDK
 Home-page: https://github.com/cardpay/python-sdk-v3.git
 Author-email: 
 License: MIT
 Project-URL: Source Code, https://github.com/cardpay/python-sdk-v3
 Project-URL: Documentation, https://integration.unlimit.com/
 Description: # Unlimit APIv3 Python SDK
@@ -27,15 +27,15 @@
         
         ```sh
         pip install git+https://github.com/cardpay/python-sdk-v3.git --upgrade
         ```
         or
         
         ```sh
-        pip install 'cardpay>=3.68.8' --upgrade
+        pip install 'cardpay>=3.73.6' --upgrade
         ```
         
         Then import the package:
         ```python
         from cardpay import *
         ```
```

