


https://chat.deepseek.com/share/ijoc30pw2hx2816pqu


1. Data Retrieval & Lookup
These are your bread and butter for pulling data from large datasets (like an income statement or a trial balance).

XLOOKUP: The modern successor to VLOOKUP. It’s more robust because it doesn't break when you insert columns.

Syntax: =XLOOKUP(lookup_value, lookup_array, return_array)

INDEX & MATCH: Still favored by many "old school" analysts for its flexibility and speed in massive models.

OFFSET: Useful for creating dynamic ranges, often used in "Scenario Managers" where you toggle between Bull, Bear, and Base cases.

2. Logical & Conditional Formulas
These allow your model to "think" and handle different accounting treatments automatically.

IF / IFS: Essential for debt schedules (e.g., "If balance > 0, calculate interest; else 0").

SUMIFS / COUNTIFS: The most used formulas for aggregating data. For example, summing all "Marketing" expenses for "Q1" only.

Syntax: =SUMIFS(sum_range, criteria_range1, criteria1, ...)

AND / OR: Usually nested inside an IF statement to check for multiple financial covenants or conditions.

3. Financial & Valuation Formulas
These do the heavy lifting for DCF (Discounted Cash Flow) models and ROI analysis.

NPV & XNPV: Calculates Net Present Value. Always use XNPV if you have specific dates for cash flows, as standard NPV assumes equal time periods.

IRR & XIRR: Calculates the Internal Rate of Return. Again, XIRR is the industry standard for precision with dates.

PMT: Used for calculating loan repayments (principal + interest).

EOMONTH: Vital for building out a monthly forecast timeline. It ensures your headers always jump to the last day of the next month.

4. Formatting & Data Cleaning
A messy model is a dangerous model.

IFERROR: Wraps around your formula to show a "0" or "-" instead of a nasty #N/A or #DIV/0!. It keeps your client-facing reports looking professional.

TEXT: Useful for combining dates and strings (e.g., "Forecast for " & TEXT(A1, "YYYY")).

EDATE: Moves a date forward or backward by a specific number of months—perfect for 3-year or 5-year projections.
