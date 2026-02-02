# Cálculo de Firmas Hash - Informática Forense

Este repositorio contiene el proyecto sobre **Cálculo de Firmas Hash**, desarrollado como parte de la formación en Técnico Superior en Ciberseguridad. El objetivo es documentar y demostrar la importancia de la integridad de los datos en el ámbito de la informática forense.

## Introducción

Una **firma hash** es un valor alfanumérico de longitud fija que representa, de forma única, el contenido de un archivo o la imagen de un dispositivo. Funciona como una "huella digital": cualquier modificación mínima en el archivo original alterará por completo el resultado del hash.



### ¿Cómo se genera un Hash?
El proceso sigue tres etapas principales:
1. **División en bloques:** El archivo se separa en fragmentos de tamaño fijo.
2. **Procesamiento:** Cada fragmento se combina mediante operaciones matemáticas (sumas, desplazamientos y permutaciones).
3. **Resultado:** Tras procesar todos los bloques, se obtiene una cadena hexadecimal única.

---

## Propósito en la Informática Forense

El uso de hashes es el pilar de la confianza en una investigación digital, permitiendo:
* **Verificar integridad:** Detectar alteraciones accidentales o intencionadas en las evidencias.
* **Prueba legal:** Demostrar ante un tribunal que la copia analizada coincide bit a bit con el original.
* **Cadena de custodia:** Mantener un registro inmutable en cada paso del análisis forense.

---

## Algoritmos y Herramientas

### Algoritmos Comunes
| Algoritmo | Estado | Uso Recomendado |
| :--- | :--- | :--- |
| **MD5** | Vulnerable | Rápido, pero propenso a colisiones. |
| **SHA-1** | Obsoleto | Ya no se considera seguro para fines forenses críticos. |
| **SHA-256** | **Seguro** | Estándar actual en la industria de la ciberseguridad. |

### Herramientas Destacadas
* **md5sum / sha256sum:** Utilidades de terminal en sistemas Linux.
* **Hashdeep:** Ideal para auditorías recursivas en directorios completos.
* **Guymager:** Herramienta gráfica para adquisición forense de discos.
* **Autopsy:** Plataforma integral que automatiza la verificación de integridad de archivos conocidos.
  
