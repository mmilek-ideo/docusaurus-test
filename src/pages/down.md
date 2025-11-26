# Button Component

Uniwersalny komponent przycisku z obsługą różnych wariantów i stanów.

## Instalacja
```bash
npm install @my-lib/button
```

## Użycie
```tsx
import { Button } from '@my-lib/button';

export function MyComponent() {
  return (
    <Button 
      variant="primary" 
      onClick={() => console.log('Clicked')}
    >
      Kliknij mnie
    </Button>
  );
}
```

## Właściwości (Props)

| Prop | Typ | Domyślnie | Opis |
|------|-----|----------|------|
| `variant` | `'primary' \| 'secondary'` | `'primary'` | Styl przycisku |
| `size` | `'sm' \| 'md' \| 'lg'` | `'md'` | Rozmiar |
| `disabled` | `boolean` | `false` | Wyłącza przycisk |
| `onClick` | `() => void` | - | Callback przy kliknięciu |

## Przykłady

### Warianty
```tsx
<Button variant="primary">Primary</Button>
<Button variant="secondary">Secondary</Button>
```

### Rozmiary
```tsx
<Button size="sm">Mały</Button>
<Button size="lg">Duży</Button>
```

## Notatki

- Komponent obsługuje dostępność (a11y)
- Klawiatura: `Enter` i `Space` aktywują przycisk