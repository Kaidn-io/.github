# Kaidn

**Fraud and abuse scoring for operators who can't justify an enterprise fraud team.**

`POST /v1/score` takes an event about a user (signup, trial start, cashout) and returns a score, a verdict (`allow`, `review` or `block`) and plain-English reasons. Rules make the decision, AI writes the explanation, and every verdict ships with evidence.

```bash
curl -X POST https://api.kaidn.io/v1/score \
  -H "x-api-key: YOUR_KEY" -H "content-type: application/json" \
  -d '{"event":"cashout","user_id":"u1","ip":"3.5.140.1","email":"x@mailinator.com"}'
```

- Website and live demo: [kaidn.io](https://kaidn.io)
- API: `api.kaidn.io`
- Self-serve signup, transparent pricing, no sales calls

The big fraud vendors built for banks. Kaidn is built and priced for everyone they ignore.
