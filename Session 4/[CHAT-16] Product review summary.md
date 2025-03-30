# [CHAT-16] Product review summary

## Input

Your task is to extract relevant information from a product review from an ecommerce site to give feedback to the Marketing department.

From the review below, extract the information relevant to product quality and price. Present your analysis according to following guidelines:
(a) Maximum length: 30 words.
(b) Language: Spanish.

<review>
A qualidade JBL é algo indiscutível, ótima qualidade de som, acabamento impecável, funcionamento perfeito. Os produtos JBL são caros, mas valem a pena, pelo preço poderiam fornecer um carregador. Uso em pequenos eventos como churrasco em família ou amigos e ela atende perfeitamente. A bateria não é das melhores, entrega umas 4 a 5 horas de uso moderado. Seu carregamento é bem rápido. O atendimento da loja me surpreendeu. Adorei a aquisição.
</review>

## Output (ChatGPT)

La calidad de sonido y acabado es excelente. El precio es alto, pero vale la pena; sin embargo, sería ideal incluir un cargador. Batería de duración media (4-5 horas).

---

## Input

Your task is to extract relevant information from a product review from an ecommerce site to give feedback to the Marketing department.

From the review below, extract the information relevant to product quality and price. Present your analysis in Spanish, as a JSON object with keys "quality" and "price".

<review>
A qualidade JBL é algo indiscutível, ótima qualidade de som, acabamento impecável, funcionamento perfeito. Os produtos JBL são caros, mas valem a pena, pelo preço poderiam fornecer um carregador. Uso em pequenos eventos como churrasco em família ou amigos e ela atende perfeitamente. A bateria não é das melhores, entrega umas 4 a 5 horas de uso moderado. Seu carregamento é bem rápido. O atendimento da loja me surpreendeu. Adorei a aquisição.
</review>

## Output (ChatGPT)

```
json

{
  "quality": "Excelente calidad de sonido, acabado impecable, funcionamiento perfecto. La batería dura entre 4 a 5 horas con uso moderado, pero el cargamento es rápido.",
  "price": "El precio es elevado, pero vale la pena. Sería ideal incluir un cargador por el precio."
}
```
---

## Input

Your task is to extract relevant information from a product review from an ecommerce site to give feedback to the Marketing department.

From the reviews below, extract the information relevant to product quality and price. Present your analysis in Spanish, as JSON objects with keys "quality" and "price". Use no more than 10 words for each key.

```
<review>
A qualidade JBL é algo indiscutível, ótima qualidade de som, acabamento impecável, funcionamento perfeito. Os produtos JBL são caros, mas valem a pena, pelo preço poderiam fornecer um carregador. Uso em pequenos eventos como churrasco em família ou amigos e ela atende perfeitamente. A bateria não é das melhores, entrega umas 4 a 5 horas de uso moderado. Seu carregamento é bem rápido. O atendimento da loja me surpreendeu. Adorei a aquisição.
</review>
```

```
<review>
Ich muss wirklich sagen das diese kleine Musikbox super klang hat und zudem was die Lautstärke betrifft top ohne Verzerrung, verbindet sich sehr schnell mit dem Handy, guter preis gute Qualität, geliefert wurde es mir in 4 Tagen.
</review>
```

## Output (ChatGPT)

```
json

[
  {
    "quality": "Excelente sonido, acabado impecable, batería de duración media.",
    "price": "Precio alto, pero vale la pena; falta cargador incluido."
  },
  {
    "quality": "Sonido excelente, volumen alto, rápida conexión.",
    "price": "Buen precio, buena calidad."
  }
]
```
