# Record
### Definición
Construye un tipo de objeto cuyas claves de propiedad son Keys y cuyos valores de propiedad son Type.

```typescript
type Message = "success" | "error" | "warning";

const messages:Record<Message,string> = {
  success:"Success message",
  error:"Error message",
  warning: "Warning message"
};

```

# Map
### Definición
Una colección de pares clave-valor que permite claves de cualquier tipo y matener el order de insercción

```typescript
const products: { name: string; items: number[] }[] = [{ name: 'Pizza', items: [] }];
const myMap = new Map();

myMap.set(products[0].id,products[0]) // Inserta un dato con su clave valor
map.get(1) => // Obtiene el valor por la clave
map.has(1) // Devuelve verdadero si la clave está presente
map.delete(1) // Elimina el dato por la clave
map.size() // Obtiene el tamaño del mapa
map.clear() // Elimina todo el mapa

mapExample.get(1).items.push(1);
mapExample.get(1).items.push(2);
mapExample.get(1).items.push(3);

for (const product of mapExample.values()) {
  product.items.sort((a: number, b: number) => b - a);
}

console.log(mapExample.values());
// [Map Iterator] { { name: 'Pizza', items: [ 3, 2, 1 ] } }

```
