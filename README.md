# Ethikcorp BusinessOS demo data

This repository is the demo document corpus for the Ethikcorp BusinessOS prototype (built by Aqionlabs.ai). The BusinessOS portal is meant to read these files from this public GitHub repository and from a matching Google Drive folder, then use them to form a BusinessBrain (chat plus dashboard charts).

Nothing in the sample-data or workflows folders is a real Ethikcorp financial, people, or pipeline figure. Those files are labelled **SAMPLE DATA for demo – not real Ethikcorp figures**.

## What is real (public website)

The `public-kb/` folder is a crawl of Ethikcorp’s public website, [ethikcorp.com](https://ethikcorp.com), taken on 14 October 2026. It is the only real company material in this corpus.

| Path | What it is |
| --- | --- |
| `public-kb/ethikcorp-kb.md` | A structured summary of the public site (services, methodology, proof points, contact, notes for each department). |
| `public-kb/index.json` | An index of the captured pages, with source URLs. |
| `public-kb/pages/*.md` | The 25 captured public pages (home, about, service pages, and blog posts), one Markdown file per page. |

This public material includes the company’s published contact details (`info@ethikcorp.com`, the public WhatsApp/phone number, the Al Qusais PO Box), the public founder biography, on-site testimonials, and “Trusted By” brand names as they appeared on the website. The knowledge-base summary already warns that logo permissions and conflicting site statistics should be verified before external use. Treat those names and claims as *public-site text*, not as confirmed facts for a pitch.

Private emails, credentials, and internal systems data were not included.

## What is sample (for charts, chat and automation analysis)

Every file below carries the header `SAMPLE DATA for demo – not real Ethikcorp figures`. Company names in these files are fictional. Pipeline owners are roles, not people. Totals are internally consistent across the four data files.

Period for the numbers: **November 2025 – October 2026**. Currency: **AED**.

| Path | What it is |
| --- | --- |
| `sample-data/monthly-revenue-by-service-line.csv` | Recognised revenue by month and by the six public service lines. Trailing-twelve-month total: AED 9,600,000. |
| `sample-data/clients.csv` | 16 fictional clients, with sector, emirate, service line, contract value and recognised TTM revenue. Recognised revenue sums to the same AED 9,600,000 and matches the service-line totals. |
| `sample-data/sales-pipeline.csv` | 22 fictional deals. Closed Won deals are TTM bookings (AED 6,862,000) and match `clients.csv` contract values for deals signed in the period. Earlier contracts that are still recognising revenue are not repeated as TTM wins. Open pipeline gross: AED 6,505,000 (weighted AED 2,397,500). |
| `sample-data/department-headcount-and-hours.csv` | October 2026 snapshot for the nine BusinessOS departments. 26 people, 4,160 hours available (headcount × 160), 3,216 hours utilised, 1,592 billable hours. |
| `sample-data/_consistency-check.json` | Machine-readable totals used to verify the four files above. Also sample, not real figures. |
| `workflows/*.md` | One current-state manual workflow description per department, with steps, illustrative time spent, and automation candidates. For Businessbots analysis only. |

The nine departments are: Sales & BD, Marketing, Consulting Delivery, Technology & AI, Finance, HR & Talent, Operations, Client Success, Legal & Compliance.

## What was deliberately left out

Internal department dashboard HTML and screenshots that had been built from live ClickUp work were **not** copied here. They mixed public-site context with internal task titles and tracker IDs, which do not belong in a public demo corpus.

Raw HTML dumps and the crawler script were also left out; the cleaned Markdown in `public-kb/` is the source to ingest.

## How the portal should read this

- **GitHub:** raw file URLs of the form `https://raw.githubusercontent.com/Jaferdecodesai/ethikcorp-businessos-demo-data/main/<path>`.
- **Google Drive:** a folder named “Ethikcorp BusinessOS Demo Data” holds the same files. File IDs and direct-download URL forms are listed in `drive-manifest.json` once that folder has been created. If a file cannot be fetched without signing in, use the GitHub raw URL; the connector used to create the folder cannot grant “anyone with the link” access by itself.

Suggested ingest order: `public-kb/ethikcorp-kb.md` and `public-kb/pages/` for company knowledge; the four CSV files for dashboard charts; `workflows/` for department Businessbot automation analysis.
