# Silent Voice API — Performance Testing
**Tool:** Apache JMeter 5.6.3
**Tester:** Eslam Waled | ITI Graduation Project

## Test Results Summary
| Test | Users | Pass Rate | APDEX |
|------|-------|-----------|-------|
| Load Test | 50 | 93.14% | 0.224 |
| Endurance Test | 10 | 100% | 0.959 |
| Spike Test | 200 peak | 100% | 0.565 |

## Key Findings
- Register fails under concurrent load — Azure DB write limit
- Voice Transcribe needs async processing
- Core APIs stable under all test types 

## How to Run
1. Open Apache JMeter 5.6.3
2. Load file from `jmx/` folder
3. Enable desired Thread Group
4. Run → Generate HTML Report
