# sanity-foundry-constants

[![npm version](https://img.shields.io/npm/v/@liiift-studio/sanity-foundry-constants.svg)](https://www.npmjs.com/package/@liiift-studio/sanity-foundry-constants)

Shared environment-driven constants for Liiift foundry Sanity Studios. Provides script configuration, discount requirement types, and an HTML description component.

## Install

```bash
npm install @liiift-studio/sanity-foundry-constants
```

## Usage

```typescript
import {
	SCRIPTS,
	SCRIPTS_OBJECT,
	DISCOUNT_REQUIREMENT_TYPES,
	DISCOUNT_REQUIREMENT_TYPES_OBJECT,
	HtmlDescription,
} from '@liiift-studio/sanity-foundry-constants'

// Script configuration list and lookup map
const allScripts = SCRIPTS
const latinConfig = SCRIPTS_OBJECT['latin']

// Discount requirement types list and lookup map
const types = DISCOUNT_REQUIREMENT_TYPES
const percentageType = DISCOUNT_REQUIREMENT_TYPES_OBJECT['percentage']

// Render HTML content in Sanity components
import React from 'react'
export const MyComponent = () => (
	<HtmlDescription content="<p>Some <strong>HTML</strong> content</p>" />
)
```

## Peer Dependencies

| Package | Version |
|---|---|
| `react` | `>=18` |
