# public.pur_vendorattributemaster

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| vendorattributeid | integer | nextval('pur_vendorattributemaster_vendorattributeid_seq'::regclass) | false | [public.stor_itemsupplierattributerating](public.stor_itemsupplierattributerating.md) |  |  |
| criteria | varchar(30) |  | true |  |  |  |
| weightage | integer |  | true |  |  |  |
| description | varchar(50) |  | true |  |  |  |
| isactive | boolean | true | false |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| authorizedon | timestamp without time zone |  | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedon | timestamp without time zone |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| inactivedate | timestamp without time zone |  | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| vendorattributemaster_pkey | PRIMARY KEY | PRIMARY KEY (vendorattributeid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| vendorattributemaster_pkey | CREATE UNIQUE INDEX vendorattributemaster_pkey ON public.pur_vendorattributemaster USING btree (vendorattributeid) |

## Relations

![er](public.pur_vendorattributemaster.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
