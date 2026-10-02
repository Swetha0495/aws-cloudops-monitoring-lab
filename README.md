# AWS CloudOps Monitoring and Incident Simulation Lab

## Project Overview
This project demonstrates hands-on AWS CloudOps practices using Amazon EC2, Amazon CloudWatch, and AWS CLI.

The objective is to monitor EC2 CPU utilization, configure threshold-based alarms, simulate incident conditions, and verify alarm state transitions.

## AWS Services and Tools
- Amazon EC2 (Amazon Linux 2023, t3.micro)
- Amazon CloudWatch Metrics and Alarms
- AWS CLI v2
- AWS CloudShell
- Linux and SSH

## Implementation
1. Launched an EC2 instance in the Stockholm region (`eu-north-1`).
2. Connected to the instance using SSH.
3. Explored EC2 CPU utilization and CPU credit metrics.
4. Created the `Swetha-EC2-High-CPU` CloudWatch alarm.
5. Configured a CPU utilization threshold greater than 70% for two datapoints within 10 minutes.
6. Inspected the alarm using AWS CLI.
7. Simulated the ALARM state using `set-alarm-state`.
8. Verified transitions from OK to ALARM and back to OK through CloudWatch alarm history.

## Results
- CloudWatch alarm successfully created.
- Manual alarm-state simulation completed.
- Alarm transitions verified through CloudWatch History.
- Alarm returned to OK after metric evaluation.

## Key Learnings
- Cloud infrastructure monitoring
- AWS CLI operations
- CloudWatch metric evaluation
- Alarm configuration and state transitions
- Incident simulation and troubleshooting

## Future Improvements
- Configure Amazon SNS notifications.
- Implement CloudWatch dashboards.
- Add infrastructure automation using Terraform.
- Explore log monitoring and incident response automation.
