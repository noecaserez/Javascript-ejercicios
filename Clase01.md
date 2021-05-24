# Ejercicios

## 1) Las galletitas de Ema:
Emanuel quiere cocinar galletitas y quiere un programa que lo ayude a saber que debe
comprar y en caso que cuente con todos los ingredientes, informar que puede cocinar las
galletas. La receta pide los siguientes ingredientes:**

- 3 huevos
- 1 barra de chocolate
- 0.5 kilos de harina
- 5 cucharadas de azucar

Los ingredientes que tiene Ema tienen que ser variables al inicio del programa que sean
faciles de editar.

```
function cocinarGalletas(huevo, choco, harina, azucar) {
  if (huevo === 3 || huevo > 3) {
    console.log("Tienes la cantidad justa de Huevos");
  } else if (huevo < 3) {
    var faltaHuevo = 3 - huevo;
    console.log("Te faltan", faltaHuevo, "Huevos");
  }
  if (choco >= 1) {
    console.log("Tienes la cantidad justa de Barra de chocolate");
  } else if (choco < 1) {
    console.log("No tienes las suficientes barras de chocolate");
  }
  if (harina >= 0.5) {
    console.log("Tienes la cantidad justa de Harina");
  } else if (harina < 0.5) {
    console.log("No tienes la cantidad suficiente de harina");
  }
  if (azucar >= 5) {
    console.log("Tienes la cantidad justa de cucharadas de azucar");
  } else if (azucar < 5) {
    var faltaAzucar = 5 - azucar;
    console.log("Te faltan", faltaAzucar, "cucharadas de Azucar");
  }
  if (huevo >= 3 && choco >= 1 && harina >= 0.5 && azucar >= 5) {
    console.log(
      "Tienes la cantidad necesaria de ingredientes. Ya puedes cocinar!"
    );
  } else {
    console.log("Necesitas ir de compras!");
  }
}

cocinarGalletas(3, 1, 0.5, 5);

    // Tienes la cantidad justa de Huevos 
    // Tienes la cantidad justa de Barra de chocolate 
    // Tienes la cantidad justa de Harina 
    // Tienes la cantidad justa de cucharadas de azucar 
    // Tienes la cantidad necesaria de ingredientes. Ya puedes cocinar!


cocinarGalletas(2, 1, 0.5, 2);
    // Te faltan 1 Huevos 
    // Tienes la cantidad justa de Barra de chocolate 
    // Tienes la cantidad justa de Harina 
    // Te faltan 3 cucharadas de Azucar 
    // Necesitas ir de compras! 

```

## 2) La tienda de ropa

Una tienda de ropa desea tener un programa que le permita calcular los aumentos a sus
prendas, para eso se tienen los datos:**

- precioDePrenda (que ronda entre los 1500 y 3000 pesos)
- porcentajeDeAumento (que ronda entre el 25-100% )
- precioFinal (precioDePrenda con el aumento agregado)

Ademas, implementar las siguiente funcionalidades:
- El programa debe informar en pantalla el precio final
- El programa debe informar en pantalla 'Precio excedido' cuando el precio final supere los $4000

## 3) Dia de paga

En una pizzeria requieren un programa que calcule cuanto cobraran neto los repartides al
final del dia (Todos cobran igual)**

Se tienen los siguientes datos obligatorios:
- repartidores (Cantidad de repartidores, puede ser cualquier numero entero)
- esFeriado (true si es Feriado, false si no)
- gananciaDelDia (Cuanto recaudo la pizzeria para distribuir a los empleados)
- porcentajeParaSueldos (Un porcentaje de gananciaDelDia)
- sueldoNetoDeRepartidor (Cuanto gana en bolsillo el repartidor)
- gananciaDelComercioFinal (Cuanto gana el comercio una vez pagados los sueldos y demas)

Se sabe que:
En feriados: porcentajeParaSueldos es del 80% de gananciaDelDia mientras que en
dias normales, es del 65%.

