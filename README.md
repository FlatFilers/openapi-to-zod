# OpenAPI to Zod Schema Converter

A TypeScript utility that converts OpenAPI/Swagger specifications into [Zod](https://github.com/colinhacks/zod) schemas. This tool helps you automatically generate type-safe validation schemas from your OpenAPI definitions.

## Features

- Converts OpenAPI schemas to Zod schemas
- Supports external schema references
- Handles circular dependencies
- Supports complex schema types including:
  - oneOf, allOf, anyOf
  - Enums
  - Arrays and Objects
  - References ($ref)
  - Custom formats (e.g., date-time)
- Generates TypeScript types from schemas
- Preserves schema descriptions

## Installation

Install the package using npm:

`npm install @flatfile/openapi-to-zod`

## Usage

1. Build the project using the build script
2. Run the converter by pointing it to your OpenAPI YAML file
3. Find your generated schemas in `generated-schemas.ts`

## Features in Detail

- **External References**: Handles `$ref` references to external YAML files
- **Circular Dependencies**: Safely handles circular references in schemas
- **Type Generation**: Automatically generates TypeScript types using Zod's inference
- **Schema Validation**: Creates runtime validation schemas using Zod
- **Description Preservation**: Maintains schema descriptions in the generated output

## Development

1. Clone the repository
2. Install dependencies
3. Make your changes
4. Build the project

## Dependencies

- `yaml`: YAML parsing
- `change-case`: Case transformation utilities
- `zod`: Schema validation library (peer dependency)
- `typescript`: TypeScript support

## License

ISC

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
