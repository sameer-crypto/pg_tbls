# public.pay_subworkingdays

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| detailsid | integer | nextval('pay_subworkingdays_detailsid_seq'::regclass) | false |  |  |  |
| masterid | integer |  | true |  |  |  |
| settingid | integer |  | true |  |  |  |
| isworkingday | boolean |  | true |  |  |  |
| isholiday | boolean |  | true |  |  |  |
| ishalfday | boolean |  | true |  |  |  |
| isalternateday | boolean |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| Pay_subWorkingdays_pkey | PRIMARY KEY | PRIMARY KEY (detailsid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| Pay_subWorkingdays_pkey | CREATE UNIQUE INDEX "Pay_subWorkingdays_pkey" ON public.pay_subworkingdays USING btree (detailsid) |

## Relations

![er](public.pay_subworkingdays.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)