# **Custom Biome Dictionary**

## **Default Configuration**
***

### `useForgeBiomeDictionaries`

With a default mod installation, `useForgeBiomeDictionaries` is set to `true` in the `common.toml` config file. This means that you are stuck with whatever biome groupings forge has autogenerated. This can be beneficial though, as it means that modded biomes are automatically discovered as long as they meet certain criteria. The downside is the inability to customize the groupings. You can use our custom biome dictionary system for more fine-grain control over biome groupings:

<br>
<br>

### **Custom Biome Dictionary Basics**

To use the custom biome dictionary system, set `useForgeBiomeDictionaries` to `false`. This will enable the base implementation which can then be modified by adding, removing, or editing the jsons in the `biome_dictionary` folder found in the config directory.

The custom dictionary system does not auto-discover modded biomes and as such requires you to manually add them where necessary.

## **Editing Dictionary JSON's**
***

### **Dictionary JSON format**

The basic format is simply a `biomes` array list containing the associated biome registry ID's
```json
{  
  "biomes": [  
  "minecraft:mushroom_field_shore",  
  "minecraft:beach",  
  "minecraft:stone_shore",  
  "minecraft:snowy_beach"  
  ]  
}
```

### **Dictionary Name**

This name of the JSON file determines the name of the dictionary name. The example above is the default `Beach.json` included with the mod. This would be used in the bee json as: `"biomeWhitelist": "tag:beach"`
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk2MDY2MDYxOF19
-->