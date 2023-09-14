# Ref
- [Youtube - Soumil Shah](https://www.youtube.com/playlist?list=PLL2hlSFBmWwzvn1BejbQ0Et32rdmnNXPa)


# Steps

## Kinesis
- Create Data Stream
- Create Data Firehose
  - Setup
    - Http Endpoint : ngrok Forwarding Address
    - S3 : Failured Data Backup
## App
- Flask
```bash
flask up
```
- ngrok
```bash
ngrok http 5000
```
## CLI Input
```bash
aws kinesis put-records --stream-name kds-test --records file://data-example.json --cli-binary-format raw-in-base64-out
```