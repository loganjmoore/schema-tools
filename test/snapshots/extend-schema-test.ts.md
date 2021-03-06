# Snapshot report for `test/extend-schema-test.ts`

The actual snapshot is saved in `extend-schema-test.ts.snap`.

Generated by [AVA](https://ava.li).

## extend existing schema creates new schema

> example object

    {
      age: 10,
      name: 'Joe',
      title: 'mr',
    }

> example version

    {
      major: 1,
      minor: 1,
      patch: 0,
    }

> new json schema

    {
      additionalProperties: false,
      description: 'Person with title',
      properties: {
        age: {
          description: 'Age in years',
          minimum: 0,
          type: 'integer',
        },
        name: {
          description: 'this person needs a name',
          format: 'name',
          minLength: 2,
          type: 'string',
        },
        title: {
          description: 'How to address this person',
          format: null,
          type: 'string',
        },
      },
      required: [
        'name',
        'age',
      ],
      title: 'Person',
      type: 'object',
    }
