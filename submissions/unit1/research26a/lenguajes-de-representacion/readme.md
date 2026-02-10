# Lenguajes de Representación Ontológica: XML, RDF y OWL

Los lenguajes de representación ontológica son fundamentales para la web semántica y la representación del conocimiento. Aunque XML, RDF y OWL se mencionan juntos frecuentemente, tienen propósitos y niveles de expresividad diferentes.

## XML (eXtensible Markup Language)

XML es un lenguaje de marcado que permite estructurar datos de forma jerárquica, pero no es propiamente un lenguaje ontológico.

**Características:**

-   Define la sintaxis y estructura de documentos mediante etiquetas personalizables
-   No tiene semántica inherente: las etiquetas no tienen significado predefinido
-   Útil para intercambio de datos entre sistemas
-   Sirve como base sintáctica para otros lenguajes (RDF/XML, OWL/XML)

**Limitaciones ontológicas:**

-   No puede expresar relaciones semánticas complejas
-   No infiere conocimiento automáticamente
-   Requiere que las aplicaciones interpreten el significado de las etiquetas

## RDF (Resource Description Framework)

RDF es el modelo fundamental de la web semántica, diseñado para describir recursos y sus relaciones.

**Estructura básica:**

-   Modelo de tripletas: **Sujeto - Predicado - Objeto**
-   Ejemplo: "Juan" - "esAutorDe" - "Libro X"
-   Utiliza URIs para identificar recursos únicamente

**Características:**

-   Proporciona semántica básica mediante vocabularios como RDFS (RDF Schema)
-   RDFS añade jerarquías de clases (rdfs:subClassOf) y propiedades (rdfs:subPropertyOf)
-   Permite describir dominios y rangos de propiedades
-   Sintaxis múltiple: RDF/XML, Turtle, N-Triples, JSON-LD

**Capacidades de RDFS:**

-   Definir clases y subclases
-   Definir propiedades y sus jerarquías
-   Especificar dominios y rangos
-   Inferencias simples basadas en jerarquías

## OWL (Web Ontology Language)

OWL extiende RDF/RDFS con mayor expresividad lógica para crear ontologías complejas.

**Niveles de expresividad:**

1.  **OWL Lite**: Expresividad limitada, más simple
2.  **OWL DL**: Basado en lógica descriptiva, balance entre expresividad y decidibilidad
3.  **OWL Full**: Máxima expresividad, pero no garantiza decidibilidad computacional

**Capacidades avanzadas:**

-   Equivalencia y disyunción de clases (owl:equivalentClass, owl:disjointWith)
-   Restricciones de cardinalidad (mínimo/máximo de propiedades)
-   Propiedades transitivas, simétricas, inversas, funcionales
-   Clases definidas por intersección, unión o complemento
-   Axiomas de igualdad y diferencia entre individuos
-   Razonamiento automático complejo
- ## Comparación y Relación

**Jerarquía de expresividad:** XML < RDF < RDFS < OWL

**Uso conjunto:**

-   XML proporciona sintaxis
-   RDF proporciona el modelo de datos y semántica básica
-   OWL añade lógica formal y razonamiento avanzado

**Aplicaciones típicas:**

-   **RDF/RDFS**: Catálogos, metadatos, grafos de conocimiento simples
-   **OWL**: Ontologías médicas (SNOMED), biomedicina (Gene Ontology), dominios que requieren inferencia compleja
