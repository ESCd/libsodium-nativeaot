# libsodium-nativeaot

[![Version](https://img.shields.io/nuget/vpre/libsodium.nativeaot)](https://www.nuget.org/packages/libsodium.nativeaot)

Pre-built binaries for [libsodium](https://libsodium.org), including static libraries for NativeAOT support.

## Features

| Property                   | Default                                                  | Description                                                                                           |
| -------------------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `$(LibSodiumRuntimeLinking)` | `true`                                                   | Toggle whether shared libraries are copied to the output directory.                                   |
| `$(LibSodiumStaticLinking)`  | `$(PublishAot) == 'true' AND $(RuntimeIdentifier) != ''` | Toggle whether `DirectPInvoke`+`NativeLibrary` items are included in the project (for Static Linking) |