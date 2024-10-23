# public.comn_termconditionmaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| termconditionid | integer | nextval('comn_termconditionmaster_termconditionid_seq'::regclass) | false |  |  |  |
| termconditionname | varchar(200) |  | true |  |  |  |
| iscative | boolean | true | false |  |  |  |
| branchid | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone |  | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| headauthorizedby | date |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| termconditionmaster_pkey | PRIMARY KEY | PRIMARY KEY (termconditionid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| termconditionmaster_pkey | CREATE UNIQUE INDEX termconditionmaster_pkey ON public.comn_termconditionmaster USING btree (termconditionid) |

## Relations

![er](public.comn_termconditionmaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)