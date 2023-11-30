# API Docs Description Guidelines

This document defines the general guidelines that you must follow while writing descriptions for API documentation.

## General Guidelines

Follow these general guidelines for descriptions:

- Avoid using passive voice if possible. See the [General Guidelines](../general) for further information on this.
- Focus on the success scenario rather than the values that are not allowed.

    ??? example
        Use a positive sentence like: ``Enter integers greater than or equal to zero`` instead of a negative one like: ``Zero and negative numbers are not allowed``.

- Keep descriptions clear, concise, complete, and correct. See the [General Guidelines](../general) for further information on this.
- Use the simple present tense, remember that the documentation describes the current operation of the API, whereas the future tense can mislead the reader into believing that the operation subject of the documentation has not been implemented yet.

## Field and Parameter descriptions

Follow these guidelines for field and parameter descriptions:

- Avoid using just the word value.

    ??? example
        The description “Value of the receivable” is ambiguous.

- If the field is boolean, start the description with ``Flag that indicates if`` or ``Flag that indicates whether``.

    ??? example
        Flag that indicates whether the receivable is valid.

- Include the ranges, allowed values, or rules when applicable.

    ??? example
        Number between 0 and 1 that represents the percentual weight of the foo. Keep in mind that the sum of the fields `foo_a` and `foo_b` must equal 1.

- Format all mentions of other fields or input values with monospace. Remember that descriptions support markdown formatting.

    ??? example
        If the flag ``has_interest`` is ``true``, the field ``interest_rate`` is required.

- Start the description with a noun that identifies the field's value.

    ??? example
        ID of the company that issues the receivable.

- Use consistent terminology across descriptions.

    ??? example
        Always use the word amount for monetary quantities.

- Use sentence capitalization and correctly capitalize known terms.
    ??? example
        URL, RESTful.

## Endpoint Descriptions and Summaries

Follow these guidelines for endpoint descriptions:

- Include a description of the return value.
    ??? example
        Returns a list of objects that represent the company foos.

- Include a general description of the parameters it receives starting with the word ``Receives``.

    ??? example
        Receives a set of configuration flags.

- Include non-trivial errors or error codes that indicate an expected outcome.

    ??? example
        Returns a Forbidden 403 error if the company foo is expired.

- Start the description with a verb.
    ??? example
        Lists all foos associated with the company.

Follow these guidelines for endpoint summaries:

- Keep the summary clear, concise, complete, and correct.
- Remember that the endpoint summary is the name that the API documentation renders for the endpoint.
- Use title casing. For example: Create Company Foo.

## Example Specification

The following OpenAPI specification serves as a sample for these guidelines:

<swagger-ui src="../assets/openapi.json"/>
