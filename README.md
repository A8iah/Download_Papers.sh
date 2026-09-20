```bash
# !/usr/bin/env bash
mkdir -p my_papers && cd my_papers

# One direct PDF link + output name
wget "<PDF_URL>" -O "<name>.pdf"
wget "<PDF_URL>" -O "<name>.pdf"

# Or a loop for many links
for url in \
  "<PDF_URL_1>" \
  "<PDF_URL_2>" ; do
  wget "$url"
done

echo "Total: $(ls -1 *.pdf 2>/dev/null | wc -l) files"
```
