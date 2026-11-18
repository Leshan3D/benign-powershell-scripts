$Host.UI.RawUI.ForegroundColor = 'Green'
Clear-Host
while ($true) {
    # Generates multiple random numbers per line to flood the screen horizontally and vertically
    $line = -join (1..12 | ForEach-Object { Get-Random -Minimum 0 -Maximum 2 })
    # Repeat the string to fill across standard terminal widths
    Write-Host ($line * 8) -NoNewline
} 
