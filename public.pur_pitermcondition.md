# public.pur_pitermcondition

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| termconditionid | integer | nextval('pur_pitermcondition_termconditionid_seq'::regclass) | false |  |  |  |
| invoiceid | integer |  | true |  |  |  |
| termconditionname | varchar(300) | NULL::character varying | true |  |  |  |
| description | varchar(500) | NULL::character varying | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| pur_pitermcondition_pky | PRIMARY KEY | PRIMARY KEY (termconditionid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| pur_pitermcondition_pky | CREATE UNIQUE INDEX pur_pitermcondition_pky ON public.pur_pitermcondition USING btree (termconditionid) |
| Index_PI_TermDet_PIID | CREATE INDEX "Index_PI_TermDet_PIID" ON public.pur_pitermcondition USING btree (invoiceid) |

## Relations

![er](public.pur_pitermcondition.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)