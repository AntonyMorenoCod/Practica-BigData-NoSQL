// Script de ejercicios prácticos MongoDB NoSQL - Práctica Big Data

// 1. Creación y uso de la base de datos
use practica_bigdata

// 2. Inserción de un único registro (Sensor en Bogotá)
db.sensores.insertOne({ sensor_id: 1, ubicacion: "Bogota", temperatura: 22.5 })

// 3. Inserción múltiple de registros (Sensores en Medellín y Cali)
db.sensores.insertMany([
  { sensor_id: 2, ubicacion: "Medellin", temperatura: 24.1 },
  { sensor_id: 3, ubicacion: "Cali", temperatura: 26.5 }
])

// 4. Consulta para visualizar todos los registros insertados
db.sensores.find()