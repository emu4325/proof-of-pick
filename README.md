# proof-of-pick

Sealed predictions with verifiable timestamps.

1. About 10 minutes before each race, the model's prediction card is sealed: only its SHA-256 is posted as a comment on that day's issue. GitHub records the comment time.
2. After all races finish, the cards are published under `picks/<date>/`.
3. Anyone can check that a card was fixed in advance: `sha256sum picks/<date>/<file>` must equal the hash in the comment posted before post time.

Cards contain only the model's own output (race, horse number, probabilities, bet flags, model fingerprint). No odds or other licensed data.

---

予想を発走前に「封印」し、後で公開して照合できるようにする記録です。発走約 10 分前にモデルの予想カードの SHA-256 だけを Issue にコメントし、全レース終了後に本文を `picks/<日付>/` に公開します。カードに含むのはモデル自身の出力だけで、オッズ等の配信データは含みません。馬券の購入を勧めるものではありません。
