New-Item -ItemType Directory -Force -Path "$HOME\the-melanin-guardians-\characters\bibles" | Out-Null
Get-Clipboard | Set-Content -Encoding UTF8 "$HOME\the-melanin-guardians-\characters\bibles\guardian-prime.md"
$p = "$HOME\the-melanin-guardians-\characters\bibles\guardian-prime.md"
"Size: $((Get-Item $p).Length) bytes"
Get-Content $p -TotalCount 5
