# 🌐 Static Website Hosting, S3 Event Notifications, and Cost Management

## 🌐 Static Website Hosting with S3
S3 can host static websites, serving HTML, CSS, JavaScript, and images.

### Steps to Host a Static Website:
1. **Bucket configuration**: Set the bucket to "public" and enable static website hosting.
2. **Index document**: Specify the index document (e.g., `index.html`).
3. **Custom error pages**: Configure custom error responses (e.g., `404.html`).
4. **Redirect rules**: Set up redirects for specific object requests.

---

## 📣 S3 Event Notifications
You can configure S3 to trigger notifications when specific events occur (e.g., object creation or deletion).

### Integration with AWS Services:
1. **AWS Lambda**: Automatically invoke functions to process objects when they are uploaded.
2. **Amazon SNS/SQS**: Notify subscribers or queue messages when events occur.

---

## 💸 S3 Cost Management
### Cost Factors:
1. **Data storage**: Charged based on the amount of data stored.
2. **Requests**: Fees for GET, PUT, and other requests.
3. **Data Transfer**: Outbound data transfers beyond AWS are charged.

### Cost Optimization:
1. **Use lifecycle policies**: Automate transitions to lower-cost storage.
2. **Choose the right storage class**: Use classes like Glacier or One Zone-IA for infrequently accessed data.
