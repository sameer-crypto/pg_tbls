# public.acc_dutyforegone_trading

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| trading_id | integer | nextval('acc_dutyforegone_trading_trading_id_seq'::regclass) | false |  |  |  |
| dutyforegoneid | integer |  | false |  |  |  |
| dutyforegonedetailid | integer |  | false |  |  |  |
| pi_id | integer |  | false |  |  |  |
| pi_detailid | integer |  | false |  |  |  |
| used_qty | numeric(15,5) | NULL::numeric | false |  |  |  |
| used_alt_qty | numeric(15,5) | NULL::numeric | true |  |  |  |
| itemid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| acc_dutyforegone_trading_pkey | PRIMARY KEY | PRIMARY KEY (trading_id) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| acc_dutyforegone_trading_pkey | CREATE UNIQUE INDEX acc_dutyforegone_trading_pkey ON public.acc_dutyforegone_trading USING btree (trading_id) |

## Relations

![er](public.acc_dutyforegone_trading.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)