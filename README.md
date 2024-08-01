# Análisis del Credit Scoring

## Autores
- Cedeño Ronald
- Pacheco Santiago

## Universidad de las Américas (UDLA)

---

## Variables con Correlación Positiva más Alta

- **credit_type_EQUI (0.602224)**:
  Esta variable tiene la correlación positiva más alta con Status. Esto significa que los préstamos asociados con el tipo de crédito EQUI tienen una mayor probabilidad de estar en default.
  
- **co-applicant_credit_type_EXP (0.155227)**:
  Esta variable muestra que si el co-aplicante tiene un tipo de crédito EXP, hay una probabilidad mayor de default. La correlación es significativa pero mucho menor que la de credit_type_EQUI.
  
- **submission_of_application_to_inst (0.128460)**:
  La presentación de la solicitud a una institución (to_inst) también está positivamente correlacionada con la probabilidad de default, aunque de manera moderada.

## Variables con Correlación Negativa más Alta

- **lump_sum_payment_not_lpsm (-0.189551)**:
  Esta variable tiene la correlación negativa más alta con Status, indicando que los préstamos que no tienen un pago único (lump sum) están menos propensos a estar en default.
  
- **Neg_ammortization_not_neg (-0.155048)**:
  Los préstamos sin amortización negativa (not_neg) tienen menos probabilidad de estar en default, lo que sugiere que los términos de amortización son un factor importante en la estabilidad del préstamo.
  
- **credit_type_CRIF (-0.134012)**:
  Los préstamos asociados con el tipo de crédito CRIF tienen menos probabilidad de estar en default, lo que contrasta con la alta correlación positiva observada con credit_type_EQUI.

## Resumen

- **DebToIncomeRatio (0.098567)**:
  El ratio de deuda a ingresos muestra una correlación positiva con el default, indicando que los prestatarios con una mayor proporción de deuda en relación con sus ingresos tienen más probabilidad de incumplir.

- **LoanToValueProperty (0.094923)**:
  El ratio préstamo-valor de la propiedad también muestra una correlación positiva, sugiriendo que a mayor ratio, mayor es el riesgo de default.

- **Credit_Score (0.004910)**:
  El puntaje de crédito tiene una correlación muy baja y positiva con el default, lo que puede ser contraintuitivo. Esto podría indicar la necesidad de revisar cómo se está utilizando el puntaje de crédito en el modelo o la calidad de los datos.

## Conclusión

Las variables **credit_type_EQUI**, **co-applicant_credit_type_EXP**, y **submission_of_application_to_inst** son las que más influyen en la probabilidad de default de un préstamo, con correlaciones positivas significativas. Por otro lado, **lump_sum_payment_not_lpsm**, **Neg_ammortization_not_neg**, y **credit_type_CRIF** tienen correlaciones negativas significativas, indicando una menor probabilidad de default.
