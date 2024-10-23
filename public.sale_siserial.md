# public.sale_siserial

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| invserialid | integer | nextval('sale_siserial_invserialid_seq'::regclass) | false |  |  |  |
| invoiceid | integer |  | true |  |  |  |
| invoicedetailid | integer |  | true |  |  |  |
| deliverynotedetailid | integer |  | true |  |  |  |
| batchid | integer |  | true |  |  |  |
| serialid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_siserial_pkey | PRIMARY KEY | PRIMARY KEY (invserialid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_siserial_pkey | CREATE UNIQUE INDEX sale_siserial_pkey ON public.sale_siserial USING btree (invserialid) |
| Index_SI_SerDet_DetID | CREATE INDEX "Index_SI_SerDet_DetID" ON public.sale_siserial USING btree (invoicedetailid) |
| Index_SI_SerDet_SIIDDetID | CREATE INDEX "Index_SI_SerDet_SIIDDetID" ON public.sale_siserial USING btree (invoiceid, invoicedetailid) |

## Relations

![er](public.sale_siserial.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)