# Product Recall Coordinator

`product-recall-coordinator` turns electronics traceability data into a controlled recall workflow, from affected-unit scope and safety risk through customer effectiveness and final reconciliation.

## Capabilities

- Content-addressed recall records with jurisdiction and approval policies
- Product, revision, lot, serial-range, and build-date scope filters
- Severity, probability, detectability, safety, risk-class, and stop-ship decisions
- Latest-location distribution mapping from ordered transactions
- Customer notification waves, channels, deadlines, and missing-contact gaps
- Contact, unit-location, and correction effectiveness rates
- Serial-level return, repair, replacement, destruction, and safe-verification reconciliation
- Timed mock-recall location metrics and duplicate detection
- Evidence-integrity, effectiveness, approval, and reconciliation closure gates
- Human-readable recall reports
- Dependency-free Node.js 18+ library and CLI

## Quick start

```bash
npm install
npm test
node src/cli.js build examples/meta.json examples/criteria.json --output recall.json
node src/cli.js validate recall.json
node src/cli.js scope examples/units.json examples/criteria.json
```

## Library API

```js
import { createRecall, scopeUnits, riskAssessment, reconcile, closureReadiness } from '@opencircuitlabs/product-recall-coordinator';
```

This software supports record control and analysis; it does not determine legal reportability or replace regulator, legal, safety, or quality authority. Recall classification, notification content, deadlines, disposition, and closure must be approved for each applicable jurisdiction.

## License

MIT. See [LICENSE](LICENSE).
