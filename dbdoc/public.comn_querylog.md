# public.comn_querylog

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| logid | integer | nextval('comn_querylog_logid_seq'::regclass) | false |  |  |  |
| querydesp | text |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone |  | true |  |  |  |

## Relations

![er](public.comn_querylog.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
