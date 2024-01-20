## Pull Request Checklist
### Code Quality
* [ ] I have checked the result of static code analysis.
* [ ] I have ensured that no new bugs were introduced.
* [ ] I have ensured that no new security issues were introduced.
* [ ] I have ensured that all security hotspots (if any) were addressed.
* [ ] I have ensured that new codes meet minimum coverage threshold.
* [ ] I have ensured that duplicates codes did not exceed the threshold.
* [ ] I have ensured that there are no new critical / blocker code smells.
* [ ] Evidence of developer testing (if applicable) is attached.

### Observability
* [ ] Best practice for logging is followed for all in/out interfaces. 
  * Process flow is observable via logs with sufficient contextual information.
* [ ] Outcome of processing for all in/out interfaces is observable via logs.
  * The following format for the outcome log is adhered: `measure response - {service}, {response_time_ms}, {process_status}, {error_code}`

### Security
* [ ] Any sensitive data (e.g: credential data, PII data) are masked in the logs
* [ ] Cryptographic related keys are not stored and logged in clear
* [ ] All inputs (all user-provided data) are validated and sanitised to prevent injection attacks
* [ ] Dependencies introduced have no known vulnerabilities exist
