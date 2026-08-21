# fix(streaming): preserve prompt_tokens_details and completion_tokens_details from dict usage chunks (#37485)

## Summary
Resolves #37485 by safely extracting `prompt_tokens_details` and `completion_tokens_details` from dictionary usage payloads as well as object instances in `_usage_chunk_calculation_helper`, ensuring that cached tokens and usage details are retained across streamed responses from Vercel AI Gateway and OpenAI-compatible endpoints.

Closes #37485
