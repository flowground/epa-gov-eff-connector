# ![LOGO](logo.png) U.S. EPA Enforcement and Compliance History Online (ECHO) - Effluent Charting and Reporting **flow**ground Connector

## Description

A generated **flow**ground connector for the U.S. EPA Enforcement and Compliance History Online (ECHO) - Effluent Charting and Reporting API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/epa.gov/eff/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:40:24+03:00

## API Description

Enforcement and Compliance History Online (ECHO) is a tool developed and maintained by EPA's Office of Enforcement and Compliance Assurance for public use.
ECHO provides integrated compliance and enforcement information for about 800,000 regulated facilities nationwide.
<BR><BR>EFF Rest Services provides the data for ECHO's Effluent Charts, a set of dynamic charts and tables of permitted effluent limits, releases, and violations over time for 
Clean Water Act (CWA) wastewater discharge permits issued under the National Pollutant Discharge Elimination System (NPDES).  See Effluent Charts Help (https://echo.epa.gov/help/reports/effluent-charts-help) for additional information.
<BR><BR>
The are 3 service end points for Efffluent Charts:  get_summary_chart, get_effluent_chart, and download_effluent_chart.
<br>
<br><b>1)</b>  Use get_summary_chart to retrieve a summary matrix of effluent parameters by effluent outfall and an overall violation status for a provided NPDES Permit and date range.
<br><b>2)</b>  Use get_effluent_chart to retrieve detailed Discharge Limit, DMR and NPDES Violation information for a provided NPDES Permit, date range, effluent paramater, or outfall.
<br><b>3)</b>  Use download_effluent_chart to generate a Comma Separated Value (CSV) file of the detailed data provided with get_effluent chart, for a provided NPDES Permit, date range, effluent paramater, or outfall.
<br>
<br>
Additional ECHO Resources:   <a href="https://echo.epa.gov/tools/web-services">Web Services</a>, <a href="https://echo.epa.gov/resources/echo-data/about-the-data">About ECHO's Data</a>, <a href="https://echo.epa.gov/tools/data-downloads">Data Downloads</a>
<br>

## Authorization

This API does not require authorization.

## Actions

### Effluent Charts Download Service

> Downloads tabular Discharge Monitoring Report (DMR) and compliance data for one NPDES permit as a CSV.

*Tags:* `Effluent Charts`

#### Input Parameters
* `p_id` - _required_ - Identifier for the service.
* `outfall` - _optional_ - Three-character code that identifies the point of discharge (e.g., pipe or outfall) for a facility. A single NPDES ID may have multiple points of discharge.
* `parameter_code` - _optional_ - Five-digit numeric code identifying the parameter. See Parameter Lookup documentation for a complete list of codes.
* `start_date` - _optional_ - The start date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with end_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `end_date` - _optional_ - The end date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with start_date. If start_date and end_date are not specified, the service will return the last three years of data.

### Effluent Charts Download Service

> Downloads tabular Discharge Monitoring Report (DMR) and compliance data for one NPDES permit as a CSV.

*Tags:* `Effluent Charts`

#### Input Parameters
* `p_id` - _required_ - Identifier for the service.
* `outfall` - _optional_ - Three-character code that identifies the point of discharge (e.g., pipe or outfall) for a facility. A single NPDES ID may have multiple points of discharge.
* `parameter_code` - _optional_ - Five-digit numeric code identifying the parameter. See Parameter Lookup documentation for a complete list of codes.
* `start_date` - _optional_ - The start date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with end_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `end_date` - _optional_ - The end date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with start_date. If start_date and end_date are not specified, the service will return the last three years of data.

### Detailed Effluent Chart Service

> Discharge Monitoring Report (DMR) data supporting each effluent chart for one NPDES permit. Includes Discharge Monitoring Reports and NPDES Violations.

*Tags:* `Effluent Charts`

#### Input Parameters
* `p_id` - _required_ - Identifier for the service.
* `outfall` - _optional_ - Three-character code that identifies the point of discharge (e.g., pipe or outfall) for a facility. A single NPDES ID may have multiple points of discharge.
* `parameter_code` - _optional_ - Five-digit numeric code identifying the parameter. See Parameter Lookup documentation for a complete list of codes.
* `start_date` - _optional_ - The start date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with end_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `end_date` - _optional_ - The end date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with start_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `output` - _optional_ - Output Format Flag.  Enter one of the following keywords:
- JSON = Data model formatted as Javascript Object Notation (default).
- JSONP = Data model formatted as Javascript Object Notation with Padding.  
- XML = Data model formatted as Extensible Markup Language.
    Possible values: JSONP, JSON, XML.
* `callback` - _optional_ - JSONP Callback.  For use with JSONP and GEOJSONP output only.  Enter a name of the function in which to wrap the JSON response.

### Detailed Effluent Chart Service

> Discharge Monitoring Report (DMR) data supporting each effluent chart for one NPDES permit. Includes Discharge Monitoring Reports and NPDES Violations.

*Tags:* `Effluent Charts`

#### Input Parameters
* `p_id` - _required_ - Identifier for the service.
* `outfall` - _optional_ - Three-character code that identifies the point of discharge (e.g., pipe or outfall) for a facility. A single NPDES ID may have multiple points of discharge.
* `parameter_code` - _optional_ - Five-digit numeric code identifying the parameter. See Parameter Lookup documentation for a complete list of codes.
* `start_date` - _optional_ - The start date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with end_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `end_date` - _optional_ - The end date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with start_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `output` - _optional_ - Output Format Flag.  Enter one of the following keywords:
- JSON = Data model formatted as Javascript Object Notation (default).
- JSONP = Data model formatted as Javascript Object Notation with Padding.  
- XML = Data model formatted as Extensible Markup Language.
    Possible values: JSONP, JSON, XML.
* `callback` - _optional_ - JSONP Callback.  For use with JSONP and GEOJSONP output only.  Enter a name of the function in which to wrap the JSON response.

### Summary Effluent Chart Service

> Summary of compliance status each outfall and parameter for one NPDES permit. Provides the current compliance status and overall compliance status for the date range of interest. This service supports the Summary Matrix on the Effluent Charts.

*Tags:* `Effluent Charts`

#### Input Parameters
* `p_id` - _required_ - Identifier for the service.
* `output` - _optional_ - Output Format Flag.  Enter one of the following keywords:
- JSON = Data model formatted as Javascript Object Notation (default).
- JSONP = Data model formatted as Javascript Object Notation with Padding.  
- XML = Data model formatted as Extensible Markup Language.
    Possible values: JSONP, JSON, XML.
* `callback` - _optional_ - JSONP Callback.  For use with JSONP and GEOJSONP output only.  Enter a name of the function in which to wrap the JSON response.
* `start_date` - _optional_ - The start date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with end_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `end_date` - _optional_ - The end date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with start_date. If start_date and end_date are not specified, the service will return the last three years of data.

### Summary Effluent Chart Service

> Summary of compliance status each outfall and parameter for one NPDES permit. Provides the current compliance status and overall compliance status for the date range of interest. This service supports the Summary Matrix on the Effluent Charts.

*Tags:* `Effluent Charts`

#### Input Parameters
* `p_id` - _required_ - Identifier for the service.
* `output` - _optional_ - Output Format Flag.  Enter one of the following keywords:
- JSON = Data model formatted as Javascript Object Notation (default).
- JSONP = Data model formatted as Javascript Object Notation with Padding.  
- XML = Data model formatted as Extensible Markup Language.
    Possible values: JSONP, JSON, XML.
* `callback` - _optional_ - JSONP Callback.  For use with JSONP and GEOJSONP output only.  Enter a name of the function in which to wrap the JSON response.
* `start_date` - _optional_ - The start date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with end_date. If start_date and end_date are not specified, the service will return the last three years of data.
* `end_date` - _optional_ - The end date (mm/dd/yyyy) for the date range of interest. Must be used in conjunction with start_date. If start_date and end_date are not specified, the service will return the last three years of data.

### ECHO CWA Parameter Lookup Service

> Look up Clean Water Act parameter codes and descriptions in the Integrated Compliance Information System - National Pollutant Discharge Elimination System (ICIS-NPDES) by code or term.

*Tags:* `Lookups`

#### Input Parameters
* `output` - _optional_ - Output Format Flag.  Enter one of the following keywords:
- JSON = Data model formatted as Javascript Object Notation (default).
- JSONP = Data model formatted as Javascript Object Notation with Padding.  
- XML = Data model formatted as Extensible Markup Language.
    Possible values: JSONP, JSON, XML.
* `callback` - _optional_ - JSONP Callback.  For use with JSONP and GEOJSONP output only.  Enter a name of the function in which to wrap the JSON response.
* `search_term` - _optional_ - Enter a partial or complete search phrase or word.
* `search_code` - _optional_ - Enter a partial or complete code value.

### ECHO CWA Parameter Lookup Service

> Look up Clean Water Act parameter codes and descriptions in the Integrated Compliance Information System - National Pollutant Discharge Elimination System (ICIS-NPDES) by code or term.

*Tags:* `Lookups`

#### Input Parameters
* `output` - _optional_ - Output Format Flag.  Enter one of the following keywords:
- JSON = Data model formatted as Javascript Object Notation (default).
- JSONP = Data model formatted as Javascript Object Notation with Padding.  
- XML = Data model formatted as Extensible Markup Language.
    Possible values: JSONP, JSON, XML.
* `callback` - _optional_ - JSONP Callback.  For use with JSONP and GEOJSONP output only.  Enter a name of the function in which to wrap the JSON response.
* `search_term` - _optional_ - Enter a partial or complete search phrase or word.
* `search_code` - _optional_ - Enter a partial or complete code value.

## License

**flow**ground :- Telekom iPaaS / epa-gov-eff-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
