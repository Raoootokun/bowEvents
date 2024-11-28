# bowEvents

弓の発射、弓のチャージ開始、弓のチャージ停止の際に発火するイベントを追加します。  

## 使い方

```javascript
import { BowEvents } from "./bowEvents";

BowEvents.shoot.subscribe(ev => {
  const { player, itemStack, projectile, chargeTick } = ev;
});

BowEvents.chargeStart.subscribe(ev => {
  const { player, itemStack } = ev;
});

BowEvents.chargeStop.subscribe(ev => {
  const { player, itemStack } = ev;
});
```
