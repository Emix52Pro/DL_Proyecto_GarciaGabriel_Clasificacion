# RESUMEN EJECUTIVO - CLASIFICACIÓN DE ENFERMEDADES EN BANANO

## OBJETIVO
Desarrollar y comparar tres modelos de transfer learning para clasificar automáticamente enfermedades en hojas de banano: Cordana, hojas Sanas y Sigatoka Negra.

## METODOLOGÍA
- **Dataset**: 900 imágenes de Data-Tesis
- **Modelos**: ResNet50, MobileNetV3-Large, EfficientNet-B0
- **Técnica**: Transfer Learning con fine-tuning
- **Métricas**: Accuracy, Precision, Recall, F1-Score, ROC-AUC

## RESULTADOS PRINCIPALES

### Tabla Comparativa Final
| Modelo | Accuracy | F1-Score | Precision | Recall | Velocidad |
|--------|----------|----------|-----------|---------|-----------|
| ResNet50 | 0.9222 | 0.9228 | 0.9237 | 0.9222 | 3065.6 |
| MobileNetV3 | 0.9444 | 0.9443 | 0.9473 | 0.9444 | 2248.6 |
| EfficientNet-B0 | 0.9222 | 0.9217 | 0.9295 | 0.9222 | 1803.2 |

## CONCLUSIONES
- **Mejor modelo**: MobileNetV3 (Accuracy: 0.9444)
- **Más rápido**: EfficientNet-B0
- **Más equilibrado**: MobileNetV3

## IMPACTO POTENCIAL
- Reducción de pérdidas agrícolas por detección temprana
- Democratización del diagnóstico fitosanitario
- Optimización de tratamientos específicos por enfermedad

## LIMITACIONES
- Dataset limitado a 900 imágenes
- Necesidad de más diversidad geográfica y temporal
- Falta de validación en campo real

## RECOMENDACIONES
- Ampliar dataset con más regiones y estaciones
- Implementar en aplicación móvil para validación
- Integrar con sistemas de recomendación de tratamientos
