# public.qlty_parametertestdetailpdi

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| parametertestdetailid | integer | nextval('qlty_parametertestdetailpdi_parametertestdetailid_seq'::regclass) | false |  |  |  |
| parameterdetailid | integer |  | true |  |  |  |
| nooftest | integer |  | true |  |  |  |
| value | numeric(17,7) |  | true |  |  |  |
| inspectionid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| qlty_parametertestdetailpdi_pkey | PRIMARY KEY | PRIMARY KEY (parametertestdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| qlty_parametertestdetailpdi_pkey | CREATE UNIQUE INDEX qlty_parametertestdetailpdi_pkey ON public.qlty_parametertestdetailpdi USING btree (parametertestdetailid) |

## Relations

![er](public.qlty_parametertestdetailpdi.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)