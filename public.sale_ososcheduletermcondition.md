# public.sale_ososcheduletermcondition

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| termconditionid | integer | nextval('sale_ososcheduletermcondition_termconditionid_seq'::regclass) | false |  |  |  |
| soid | integer |  | true |  |  |  |
| scheduleno | integer |  | true |  |  |  |
| termconditionname | varchar(300) | NULL::character varying | true |  |  |  |
| description | varchar(400) | NULL::character varying | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| sale_ososcheduletermcondition_pkey | PRIMARY KEY | PRIMARY KEY (termconditionid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| sale_ososcheduletermcondition_pkey | CREATE UNIQUE INDEX sale_ososcheduletermcondition_pkey ON public.sale_ososcheduletermcondition USING btree (termconditionid) |

## Relations

![er](public.sale_ososcheduletermcondition.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)