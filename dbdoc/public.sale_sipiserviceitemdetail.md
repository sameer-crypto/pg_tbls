# public.sale_sipiserviceitemdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| serviceitemdetailid | integer | nextval('sale_sipiserviceitemdetail_serviceitemdetailid_seq'::regclass) | false |  |  |  |
| invoiceid | integer |  | true |  |  |  |
| itemid | integer |  | true |  |  |  |
| serviceamount | numeric(18,5) |  | true |  |  |  |
| issales | boolean | false | true |  |  |  |

## Relations

![er](public.sale_sipiserviceitemdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)