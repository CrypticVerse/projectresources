## Implementation in your mod
To implement this mod, follow the steps below.

### Maven
Add the maven repo for CrypticVerse's Resources
```gradle
repositories {
    maven { url = "https://raw.githubusercontent.com/CrypticVerse/projectresources/master/maven" }
}
```

### Implementation
```gradle
modImplementation "net.crypticverse.betterbiomes:BetterBiomes-Fabric:${betterbiomes_version}-${mc_verison}"
implementation fg.deobf("net.crypticverse.betterbiomes:BetterBiomes-Forge:${betterbiomes_version}-${mc_verison}")
```

### A quick note
If you are using an implementation, you need to include the maven for other project resources.
```gradle
// Fabric:
maven {url = "https://maven.shedaniel.me"}
maven {url = "https://maven.minecraftforge.net"}
maven {url = "https://maven.terraformersmc.com"}

// Forge
maven {url = "https://maven.blamejared.com"}
mavezzn {url = "https://maven.shedaniel.me"}
```

