# public.prod_bcratecheckcontroldetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| transactiondetailid | integer | nextval('prod_bcratecheckcontroldetail_transactiondetailid_seq'::regclass) | false |  |  |  |
| transactionid | integer |  | true |  |  |  |
| stageid | integer |  | true |  |  |  |
| rateperunit | numeric(15,5) |  | true |  |  |  |

## Relations

![er](public.prod_bcratecheckcontroldetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)