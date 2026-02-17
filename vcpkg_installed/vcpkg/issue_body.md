Package: openal-soft:arm64-osx@1.23.1#1

**Host Environment**

- Host: arm64-osx
- Compiler: AppleClang 17.0.0.17000013
- CMake Version: 3.31.10
-    vcpkg-tool version: 2025-12-16-44bb3ce006467fc13ba37ca099f64077b8bbf84d
    vcpkg-scripts version: e5a1490e14 2026-02-14 (3 days ago)

**To Reproduce**

`vcpkg install `

**Failure logs**

```
Downloading https://github.com/kcat/openal-soft/archive/1.23.1.tar.gz -> kcat-openal-soft-1.23.1.tar.gz
Successfully downloaded kcat-openal-soft-1.23.1.tar.gz
-- Extracting source /Users/nishio/Documents/Azura/Particles/SimulationSkeleton_new/vcpkg/downloads/kcat-openal-soft-1.23.1.tar.gz
-- Applying patch c12ada68951ea67a59bef7d4fcdf22334990c12a.patch
-- Using source at /Users/nishio/Documents/Azura/Particles/SimulationSkeleton_new/vcpkg/buildtrees/openal-soft/src/1.23.1-180897dbaa.clean
-- Configuring arm64-osx
-- Building arm64-osx-dbg
-- Building arm64-osx-rel
-- Fixing pkgconfig file: /Users/nishio/Documents/Azura/Particles/SimulationSkeleton_new/vcpkg/packages/openal-soft_arm64-osx/lib/pkgconfig/openal.pc
CMake Error at scripts/cmake/vcpkg_find_acquire_program.cmake:201 (message):
  Could not find pkg-config.  Please install it via your package manager:

      brew install pkg-config
Call Stack (most recent call first):
  scripts/cmake/vcpkg_fixup_pkgconfig.cmake:193 (vcpkg_find_acquire_program)
  buildtrees/versioning_/versions/openal-soft/8000875d5dc94ae2b77e940befb113655efd55c1/portfile.cmake:102 (vcpkg_fixup_pkgconfig)
  scripts/ports.cmake:206 (include)



```

**Additional context**

<details><summary>vcpkg.json</summary>

```
{
  "name": "particlelife",
  "version": "0.0.1",
  "dependencies": [
    {
      "name": "imgui",
      "version>=": "1.89.7"
    },
    {
      "name": "sfml",
      "version>=": "2.6.1"
    },
    {
      "name": "imgui-sfml",
      "version>=": "2.6"
    }
  ],
  "builtin-baseline": "b8a9371ae5a920b021132f443cc5658e82ac7551"
}

```
</details>
