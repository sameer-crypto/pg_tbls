# public.sale_sogstdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| sogstdetailid | integer | nextval('sale_sogstdetail_sogstdetailid_seq'::regclass) | false |  |  |  |
| soid | integer |  | true |  |  |  |
| sodetailid | integer |  | true |  |  |  |
| taxtemplateid | integer |  | true |  |  |  |
| taxid | integer |  | true |  |  |  |
| igstrate | numeric(6,3) |  | true |  |  |  |
| cgstrate | numeric(6,3) |  | true |  |  |  |
| sgstrate | numeric(6,3) |  | true |  |  |  |
| igstamount | numeric(17,5) | 0 | true |  |  |  |
| cgstamount | numeric(17,5) | 0 | true |  |  |  |
| sgstamount | numeric(17,5) | 0 | true |  |  |  |
| gsttotal | numeric(255,0) |  | true |  |  |  |
| itemtotal | numeric |  | true |  |  |  |
| itemid | integer |  | true |  |  |  |
| gst_asseablevalue | numeric(17,5) |  | true |  |  |  |
| gstcessrate | numeric(5,2) |  | true |  |  |  |
| gstcessamount | numeric(17,5) | 0 | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_sogstdetail_pkey | PRIMARY KEY | PRIMARY KEY (sogstdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_sogstdetail_pkey | CREATE UNIQUE INDEX sale_sogstdetail_pkey ON public.sale_sogstdetail USING btree (sogstdetailid) |
| Index_SO_GSTDet_SOID | CREATE INDEX "Index_SO_GSTDet_SOID" ON public.sale_sogstdetail USING btree (soid) |

## Relations

![er](public.sale_sogstdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
