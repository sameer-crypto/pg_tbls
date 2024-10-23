# public.stor_storeissuebatchdetail

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| batchdetailid | integer | nextval('stor_storeissuebatchdetail_batchdetailid_seq'::regclass) | false |  |  |  |
| issuedetailid | integer |  | false |  |  |  |
| batchid | integer |  | true |  |  |  |
| baseqty | numeric(15,5) |  | true |  |  |  |
| altqty | numeric(15,5) |  | true |  |  |  |
| issueid | integer |  | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| stor_storissuebatchdetail_pkey | PRIMARY KEY | PRIMARY KEY (batchdetailid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| stor_storissuebatchdetail_pkey | CREATE UNIQUE INDEX stor_storissuebatchdetail_pkey ON public.stor_storeissuebatchdetail USING btree (batchdetailid) |
| storeissuebatch_batchid | CREATE INDEX storeissuebatch_batchid ON public.stor_storeissuebatchdetail USING btree (batchid) |
| storeissuebatch_issuedetailid | CREATE INDEX storeissuebatch_issuedetailid ON public.stor_storeissuebatchdetail USING btree (issuedetailid) |

## Triggers

| Name | Definition |
| ---- | ---------- |
| storeissuebatchdetail_trg_checkstock | CREATE TRIGGER storeissuebatchdetail_trg_checkstock BEFORE INSERT ON public.stor_storeissuebatchdetail FOR EACH ROW EXECUTE FUNCTION trg_checkstock() |

## Relations

![er](public.stor_storeissuebatchdetail.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)