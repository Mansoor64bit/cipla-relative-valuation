Cipla — Relative (Comparable Company) Valuation
A quick, formula-driven relative valuation of Cipla Ltd. built against 9 listed Indian pharma peers, using EV/Revenue, EV/EBITDA, and P/E multiples.
![Relative Valuation Summary](/01_relative_valuation_summary.png)
What this is
This model answers one question: based on how the market prices similar pharma companies, is Cipla trading cheap or expensive?
It pulls trading multiples (EV/Revenue, EV/EBITDA, P/E) for 9 comparable Indian pharmaceutical companies, works out the median for each multiple, applies that median to Cipla's own Revenue/EBITDA/Net Income, and backs into an "implied" share price for Cipla under each method. That implied price is then compared to Cipla's actual market price to flag it as undervalued or overvalued.
Files
File	Description
`Cipla_Relative_Valuation_Model.xlsx`	The financial model — two tabs, fully formula-linked
`Report.docx`	Written summary of the methodology, numbers, and conclusion
`screenshots/`	Visual snapshots of the model
How the model is built
Tab 1 — `Relative Valuation`
Comparable company table: Share Price, Shares Outstanding, Equity Value, Net Debt, Enterprise Value, Revenue, EBITDA, Net Income, and the three resulting multiples (EV/Revenue, EV/EBITDA, P/E) for each peer.
Summary stats across peers: High, 75th Percentile, Average, Median, 25th Percentile, Low for each multiple.
A "Cipla Comparable Valuation" block that applies the peer median multiple to Cipla's own financials to derive an implied Enterprise Value → implied Market Value → implied Value per Share, for all three methods.
A final flag comparing the implied share price to Cipla's actual share price (`Undervalued` / `Overvalued`).
Tab 2 — `Raw Data - screener`
Source data for 30 Indian pharma companies (share price, shares outstanding, market cap, debt, cash, net debt, EV, sales, EBITDA, net profit) — pulled from screener.in-style fundamentals. The 9 peer companies used in the valuation tab are drawn from this larger list.
Every valuation number is a live formula referencing the raw data tab — change a peer's price or financials on the raw data sheet, and the entire valuation cascades through automatically. Nothing is hardcoded.
Peer set used
Sun Pharma, Divi's Labs, Torrent Pharma, Zydus Lifesciences, Lupin, Mankind Pharma, Dr Reddy's Labs, Laurus Labs, Aurobindo Pharma.
Key output (at the point of this snapshot)
Multiple	Peer Median	Implied Value/Share (Cipla)	Actual Price	Verdict
EV/Revenue	7.1x	₹2,489	₹1,432	Undervalued
EV/EBITDA	25.2x	₹1,660	₹1,432	Overvalued
P/E	37.7x	₹1,565	₹1,432	Overvalued
Two out of three methods (EV/EBITDA and P/E) suggest Cipla is trading slightly rich to its peer median; EV/Revenue tells the opposite story, largely because Cipla's revenue base is large relative to its EV compared to peers. See `Report.docx` for the full write-up and caveats.
How to use it
Open `Cipla_Relative_Valuation_Model.xlsx` in Excel or Google Sheets.
Update figures on the `Raw Data - screener` tab as fresher market data comes in (price changes daily; financials change quarterly).
The `Relative Valuation` tab recalculates automatically.
Add or remove peers by adjusting which raw-data rows feed the peer table (row references in columns B–K).
Disclaimer
This is an educational/illustrative valuation exercise, not investment advice. Comparable company analysis is sensitive to peer selection, and a small peer set (9 companies) means the median can shift materially if peers are added or removed. Cross-check with a DCF or other valuation method before drawing conclusions.
