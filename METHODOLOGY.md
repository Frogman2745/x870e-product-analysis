# Methodology

## Decision question

When is the ROG Crosshair X870E Hero's premium defensible while premium X870E competitors discount aggressively?

## Comparison set

- ASUS ROG Crosshair X870E Hero
- MSI MPG X870E Carbon WiFi
- Gigabyte X870E AORUS Master

All three products use AMD's AM5 / X870E platform and occupy the premium ATX motherboard segment. The model is intentionally bounded to this three-product set.

## Data hierarchy

1. Manufacturer product and specification pages control hardware specifications.
2. Manufacturer stores are preferred for direct and promotional price observations.
3. A named retailer is used when no direct observed price is captured.
4. Every price observation is stored with its source and capture date.

## Category scoring

Positive feature inputs use a relative-to-best index within the three-product comparison:

```text
feature score = product value / highest observed value × 100
```

The workbook's price score uses an inverse relative-price index:

```text
price score = lowest observed price / product observed price × 100
```

That makes the lowest observed price score 100 and reduces the score as price rises. It is a comparative value input—not an estimate of willingness to pay.

### Performance / OC

- 55% advertised DDR5 overclocking ceiling
- 45% VCORE phase count

### Expansion

- 55% total M.2 slots
- 45% PCIe 5.0 M.2 slots

### Connectivity

- 35% USB4 port count
- 30% LAN port count
- 35% maximum LAN speed

### DIY experience

Named tool-less or installation-oriented feature count divided by the highest count in the comparison set.

### Software / AI

Named AI or automated-tuning feature count divided by the highest count in the comparison set.

### Price / value

Inverse relative-price score based on observed current price on the capture date.

## Persona weights

| Persona | Performance / OC | Expansion | Connectivity | DIY | Software / AI | Price / value |
|---|---:|---:|---:|---:|---:|---:|
| Competitive Gamer | 30% | 10% | 15% | 15% | 15% | 15% |
| Enthusiast / Overclocker | 35% | 20% | 10% | 10% | 20% | 5% |
| Creator / AI Developer | 20% | 30% | 25% | 5% | 10% | 10% |
| Premium DIY Builder | 20% | 15% | 15% | 30% | 10% | 10% |

Each persona score is a `SUMPRODUCT` of the six category scores and its 100% weight set.

## Price sensitivity

The sensitivity sheet changes only the ROG scenario price—$599.99, $549.99, $499.99, and $449.99. All non-price ROG inputs remain fixed. This isolates how a channel-price decision changes modeled segment fit without implying that the product's hardware changed.

## Caveats

- Advertised specifications are not substitutes for independent performance testing.
- Counted feature proxies do not measure quality, usability, firmware maturity, or reliability.
- Promotional and marketplace prices can change quickly.
- The model does not cover every X870E board or adjacent price tier.
- A different but reasonable weight set can produce a different result; that is expected and is part of the model's purpose.

## Recommended next research

1. Add channel price history across major retailers.
2. Tag recurring customer-review praise and complaints into a voice-of-customer matrix.
3. Add adjacent X870E variants to assess portfolio overlap and cannibalization.
4. Test persona weights with interviews rather than treating them as fixed truths.

