# Completar-Pago-Mercadopago-LambdaAWS

## COMPLETAR UN PAGO MEDIANTE UNA FUNCION LAMBDA DE AWS


#### Endpoint

`Url` : <https://52dkl2m34e.execute-api.us-east-1.amazonaws.com/default/completar-pago-m>

#### Ejemplo del body

```json
{
    "token":"5c8114f99a1f3bd3786700c0eb85ea10",
    "issuer_id":"12347",
    "payment_method_id":"master",
    "transaction_amount":60,
    "installments":1,
    "payer":{
        "email":"myemail@gmail.com",
        "identification":{
            "type":"DNI",
            "number":"12345678"
        }
    }
}

```

#### Ejemplo de Response

```json
{
    "statusCode": 200,
    "body": {
        "id": 1311273592,
        "date_created": "2023-01-16T18:20:45.998-04:00",
        "date_approved": "2023-01-16T18:20:46.143-04:00",
        "date_last_updated": "2023-01-16T18:20:46.143-04:00",
        "date_of_expiration": null,
        "money_release_date": "2023-01-30T18:20:46.143-04:00",
        "money_release_status": null,
        "operation_type": "regular_payment",
        "issuer_id": "12551",
        "payment_method_id": "visa",
        "payment_type_id": "credit_card",
        "payment_method": {
            "id": "visa",
            "type": "credit_card"
        },
        "status": "approved",
        "status_detail": "accredited",
        "currency_id": "PEN",
        "description": null,
        "live_mode": false,
        "sponsor_id": null,
        "authorization_code": null,
        "money_release_schema": null,
        "taxes_amount": 0,
        "counter_currency": null,
        "brand_id": null,
        "shipping_amount": 0,
        "build_version": "2.127.2",
        "pos_id": null,
        "store_id": null,
        "integrator_id": null,
        "platform_id": null,
        "corporation_id": null,
        "collector_id": 535606744,
        "payer": {
            "first_name": null,
            "last_name": null,
            "email": "test_user_80507629@testuser.com",
            "identification": {
                "number": "32659430",
                "type": "DNI"
            },
            "phone": {
                "area_code": null,
                "number": null,
                "extension": null
            },
            "type": null,
            "entity_type": null,
            "id": "681906600"
        },
        "marketplace_owner": null,
        "metadata": {},
        "additional_info": {
            "available_balance": null,
            "nsu_processadora": null,
            "authentication_code": null
        },
        "order": {},
        "external_reference": null,
        "transaction_amount": 50,
        "transaction_amount_refunded": 0,
        "coupon_amount": 0,
        "differential_pricing_id": null,
        "financing_group": null,
        "deduction_schema": null,
        "installments": 1,
        "transaction_details": {
            "payment_method_reference_id": null,
            "net_received_amount": 46.58,
            "total_paid_amount": 50,
            "overpaid_amount": 0,
            "external_resource_url": null,
            "installment_amount": 50,
            "financial_institution": null,
            "payable_deferral_period": null,
            "acquirer_reference": null
        },
        "fee_details": [
            {
                "type": "mercadopago_fee",
                "amount": 3.42,
                "fee_payer": "collector"
            }
        ],
        "charges_details": [],
        "captured": true,
        "binary_mode": false,
        "call_for_authorize_id": null,
        "statement_descriptor": "PEARSON",
        "card": {
            "id": null,
            "first_six_digits": "400917",
            "last_four_digits": "6176",
            "expiration_month": 11,
            "expiration_year": 2025,
            "date_created": "2023-01-16T18:20:46.000-04:00",
            "date_last_updated": "2023-01-16T18:20:46.000-04:00",
            "cardholder": {
                "name": "Juan lopes",
                "identification": {
                    "number": "12345678",
                    "type": "DNI"
                }
            }
        },
        "notification_url": null,
        "refunds": [],
        "processing_mode": "aggregator",
        "merchant_account_id": null,
        "merchant_number": null,
        "point_of_interaction": {
            "type": "UNSPECIFIED",
            "business_info": {
                "unit": "online_payments",
                "sub_unit": "sdk"
            }
        }
    }
}

```

#### Imagen de Response

![obj-mercadopago](https://user-images.githubusercontent.com/93224951/212775396-50fcd4a1-02f3-4719-873b-aac5d78f7b20.jpg)

