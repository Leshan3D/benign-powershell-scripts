# matrix.ps1
$Host.UI.RawUI.ForegroundColor = 'Green'
Clear-Host
while ($true) {
    # Generate a random string of 118 binary digits per line
    $line = -join (Get-Random -InputObject 0, 1 -Count 118)
    Write-Host $line
    Start-Sleep -Milliseconds 33
}