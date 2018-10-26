Scripts for receiving git hooks via husky. Most generally useful file is `hook-pre-push-wrapper.sh`.

`.huskyrc.json`:

```json
{
  "hooks": {
    "post-commit": "bash dev/hooks/post-commit-no-enterprise.sh",
    "pre-push": "bash dev/hooks/util/hook-pre-push-wrapper.sh dev/hooks/check-no-enterprise.sh"
  }
}
```
