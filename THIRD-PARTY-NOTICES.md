# Third-party notices

Dune Pulse is published by FerreTech Interactive LLC under its own terms ([LICENSE.md](https://github.com/DuneDocker-app/dune-pulse/blob/main/LICENSE.md)). It includes, or is based on, the third-party work listed below, under that work's own license.

## Microsoft .NET Desktop Runtime

Dune Pulse runs on Microsoft's .NET Desktop Runtime 10. Setup downloads it from Microsoft, unchanged, only when it's missing and you agree. It is Microsoft's software under Microsoft's license for .NET ([dotnet/core LICENSE](https://github.com/dotnet/core/blob/main/LICENSE.TXT)).

The Windows bindings built into the app for the Blueprints 3D view (`Microsoft.Windows.SDK.NET`, `WinRT.Runtime`, the C#/WinRT projection of the Windows SDK) are Microsoft's, under the MIT License ([microsoft/CsWinRT LICENSE](https://github.com/microsoft/CsWinRT/blob/master/LICENSE)).

## Blueprint Studio renderer (TOOLS › Blueprints, 3D view)

The 3D view shows bases with Blueprint Studio's renderer and page script, as built for the Dune Docker Blueprint Installer (`src/DunePulse/Assets/BlueprintViewer/studio-viewer.js`, unchanged but for one line added at the end that hands Dune Pulse's page the renderer, and its storey lookup cached for Dune Pulse's read-only view so that large bases load faster; where it came from is in the README beside it). Blueprint Studio and the installer are part of the Dune Docker project, by Red-Blink, the same project as Dune Pulse; their use here was agreed on 2026-11-25. The renderer downloads each piece's model from blueprints.dunedocker.app only after you turn the 3D view on.

It includes three.js, whose notice is kept inline in that file:

```
The MIT License

Copyright © 2010-2026 three.js authors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

## Draco 3D decoder (TOOLS › Blueprints, 3D view)

`draco_wasm_wrapper.js` and `draco_decoder.wasm` unpack the compressed piece models. Draco is Copyright 2017 The Draco Authors (Google), under the Apache License, Version 2.0 ([google/draco LICENSE](https://github.com/google/draco/blob/main/LICENSE)). The files are included unchanged.

## Microsoft Edge WebView2 SDK (TOOLS › Blueprints, 3D view)

The 3D view runs in Microsoft Edge WebView2. Dune Pulse includes the WebView2 SDK's libraries and its `WebView2Loader.dll`, unchanged; the WebView2 Runtime itself is Windows' own and is not included.

```
Copyright (C) Microsoft Corporation. All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

   * Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.
   * Redistributions in binary form must reproduce the above
copyright notice, this list of conditions and the following disclaimer
in the documentation and/or other materials provided with the
distribution.
   * The name of Microsoft Corporation, or the names of its contributors
may not be used to endorse or promote products derived from this
software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
