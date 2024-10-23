# public.pay_adjustmentvoucer_emp_dedu

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| docdetailiddedu | integer | nextval('pay_adjustmentvoucer_emp_dedu_docdetailiddedu_seq'::regclass) | false |  |  |  |
| docid | integer |  | false |  |  |  |
| pay_head_id | integer |  | false |  |  |  |
| more_dedu | numeric(15,5) |  | true |  |  |  |
| less_dedu | numeric(15,5) |  | true |  |  |  |
| remarks | varchar |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pay_adjustmentvoucer_emp_dedu_pkey | PRIMARY KEY | PRIMARY KEY (docdetailiddedu) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pay_adjustmentvoucer_emp_dedu_pkey | CREATE UNIQUE INDEX pay_adjustmentvoucer_emp_dedu_pkey ON public.pay_adjustmentvoucer_emp_dedu USING btree (docdetailiddedu) |

## Relations

![er](public.pay_adjustmentvoucer_emp_dedu.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)