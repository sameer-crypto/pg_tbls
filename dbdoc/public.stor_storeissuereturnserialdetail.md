# public.stor_storeissuereturnserialdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| serialdetailid | integer | nextval('stor_storeissuereturnserialdetail_serialdetailid_seq'::regclass) | false |  |  |  |
| returndetailid | integer |  | true |  |  |  |
| issuereturnid | integer |  | true |  |  |  |
| serialid | bigint |  | true |  |  |  |
| batchid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| stor_storeissuereturnserialdetail_pkey | PRIMARY KEY | PRIMARY KEY (serialdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| stor_storeissuereturnserialdetail_pkey | CREATE UNIQUE INDEX stor_storeissuereturnserialdetail_pkey ON public.stor_storeissuereturnserialdetail USING btree (serialdetailid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| serialhistorydata | CREATE TRIGGER serialhistorydata BEFORE INSERT ON public.stor_storeissuereturnserialdetail FOR EACH ROW EXECUTE FUNCTION tgr_serialhistory() |

## Relations

![er](public.stor_storeissuereturnserialdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
