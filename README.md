# sp-theme-provider

A simple React utility and hook to get and use the SharePoint theme.

## Usage

In your root web part, use the `SpThemeProvider` component to wrap most of your
components. The children of this component can leverage the SharePoint hook.

```typescript
<SpThemeProvider observer={this} serviceScope={this.context.serviceScope}>
  {children}
</SpThemeProvider>
```

Use the `useSpTheme` hook to get the `IReadonlyTheme` in your component.

```typescript
const theme = useSpTheme();
```
