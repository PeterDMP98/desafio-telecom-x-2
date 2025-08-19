# 📊 Desafío Telecom X – Parte 2

Este proyecto corresponde al **Desafío Telecom X parte 2**, donde se aplican técnicas de **estadística, regresión lineal y machine learning** en un caso real de negocio: la predicción de cancelación de clientes (*churn*).

---

## 🚀 Objetivos

- Analizar los datos de clientes de una empresa de telecomunicaciones.
- Identificar variables clave que influyen en la cancelación (*churn*).
- Construir modelos predictivos con distintos algoritmos.
- Comparar su desempeño y obtener conclusiones prácticas para la empresa.

---

## 📂 Estructura del Proyecto

- `telecomX_2.csv` → Dataset base.
- `notebook.ipynb` o `main.py` → Código de análisis y modelado.
- `results/` → Carpeta con:
  - Gráficos generados (importancia de variables).
  - Archivos CSV con coeficientes/variables más relevantes.
- `README.md` → Documentación del proyecto.

---

## 🛠️ Tecnologías

- Python 3.x  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn (Regresión Logística, Random Forest, KNN, SVM)  
- Imbalanced-learn (SMOTE para balanceo de clases)  

---

## 📈 Modelos Evaluados

1. **Regresión Logística**
   - Modelo interpretable, útil para explicar tendencias.
   - Destaca la influencia de `InternetService_Fiber optic` y `Charges_Monthly`.

2. **Random Forest**
   - Mejor desempeño en relaciones no lineales.
   - Variables clave: `PaymentMethod_Electronic check`, `tenure`, `Charges_Total`.

3. **KNN (Permutation Importance)**
   - Captura proximidad entre clientes.
   - Importantes: `Charges_Total`, `tenure`, `Contract`.

4. **SVM (opcional)**
   - Similar a la logística, refuerza la importancia de fibra óptica y facturación.

---

## 📊 Principales Conclusiones

- Los **determinantes del churn** son:  
  `tenure`, `tipo de contrato`, `método de pago`, `cargos mensuales/totales` y `servicio de internet`.  

- **Modelos **:  
  - Para **interpretabilidad**: Logística / SVM.  
  - Para **robustez y precisión**: Random Forest.  
  - Para **relaciones locales**: KNN.  

---

## 🎯 Recomendaciones Estratégicas

1. **Ofertas de permanencia**: migrar clientes de contratos mes a mes a planes anuales.  
2. **Paquetes de valor agregado**: incluir soporte técnico y seguridad en línea.  
3. **Campañas tempranas**: foco en clientes nuevos con facturación alta.  
4. **Mejorar experiencia de pago**: incentivar el uso de tarjetas/débito en lugar de cheque electrónico.  
5. **Atención diferenciada**: monitoreo activo a usuarios de fibra óptica.  

