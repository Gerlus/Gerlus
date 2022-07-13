---- Minecraft Crash Report ----
// Would you like a cupcake?

Time: 7/13/22 12:04 PM
Description: Exception in server tick loop

java.lang.NoSuchMethodError: net.minecraft.entity.projectile.ProjectileHelper.func_221273_a(Lnet/minecraft/entity/Entity;Lnet/minecraft/util/math/vector/Vector3d;Lnet/minecraft/util/math/vector/Vector3d;Lnet/minecraft/util/math/AxisAlignedBB;Ljava/util/function/Predicate;D)Lnet/minecraft/util/math/EntityRayTraceResult;
	at org.infernalstudios.infernalexp.network.WhipReachPacket.lambda$handle$1(WhipReachPacket.java:73) ~[infernalexp:2.5.0] {re:classloading}
	at net.minecraftforge.fml.network.NetworkEvent$Context.enqueueWork(NetworkEvent.java:215) ~[forge:?] {re:classloading}
	at org.infernalstudios.infernalexp.network.WhipReachPacket.handle(WhipReachPacket.java:62) ~[infernalexp:2.5.0] {re:classloading}
	at net.minecraftforge.fml.network.simple.IndexedMessageCodec.lambda$tryDecode$3(IndexedMessageCodec.java:128) ~[forge:?] {re:classloading}
	at java.util.Optional.ifPresent(Optional.java:159) ~[?:1.8.0_292] {}
	at net.minecraftforge.fml.network.simple.IndexedMessageCodec.tryDecode(IndexedMessageCodec.java:128) ~[forge:?] {re:classloading}
	at net.minecraftforge.fml.network.simple.IndexedMessageCodec.consume(IndexedMessageCodec.java:162) ~[forge:?] {re:classloading}
	at net.minecraftforge.fml.network.simple.SimpleChannel.networkEventListener(SimpleChannel.java:80) ~[forge:?] {re:mixin,re:classloading}
	at net.minecraftforge.eventbus.EventBus.doCastFilter(EventBus.java:247) ~[eventbus-4.0.0.jar:?] {}
	at net.minecraftforge.eventbus.EventBus.lambda$addListener$11(EventBus.java:239) ~[eventbus-4.0.0.jar:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:302) ~[eventbus-4.0.0.jar:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:283) ~[eventbus-4.0.0.jar:?] {}
	at net.minecraftforge.fml.network.NetworkInstance.dispatch(NetworkInstance.java:86) ~[forge:?] {re:classloading}
	at net.minecraftforge.fml.network.NetworkHooks.lambda$onCustomPayload$1(NetworkHooks.java:91) ~[forge:?] {re:classloading}
	at java.util.Optional.map(Optional.java:215) ~[?:1.8.0_292] {}
	at net.minecraftforge.fml.network.NetworkHooks.onCustomPayload(NetworkHooks.java:91) ~[forge:?] {re:classloading}
	at net.minecraft.network.play.ServerPlayNetHandler.func_147349_a(ServerPlayNetHandler.java:1413) ~[?:?] {re:mixin,pl:accesstransformer:B,re:classloading,pl:accesstransformer:B,pl:mixin:APP:endergetic.mixins.json:ServerPlayNetHandlerMixin,pl:mixin:APP:tombstone.mixins.json:ServerPacketMixin,pl:mixin:A}
	at net.minecraft.network.play.client.CCustomPayloadPacket.func_148833_a(CCustomPayloadPacket.java:42) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.network.play.client.CCustomPayloadPacket.func_148833_a(CCustomPayloadPacket.java:12) ~[?:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.network.PacketThreadUtil.func_225383_a(SourceFile:21) ~[?:?] {re:classloading,xf:OptiFine:default}
	at net.minecraft.util.concurrent.TickDelayedTask.run(SourceFile:18) ~[?:?] {re:classloading}
	at net.minecraft.util.concurrent.ThreadTaskExecutor.func_213166_h(SourceFile:144) ~[?:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:computing_frames,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.util.concurrent.RecursiveEventLoop.func_213166_h(SourceFile:23) ~[?:?] {re:mixin,re:computing_frames,re:classloading}
	at net.minecraft.server.MinecraftServer.func_213166_h(MinecraftServer.java:734) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.server.MinecraftServer.func_213166_h(MinecraftServer.java:159) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.util.concurrent.ThreadTaskExecutor.func_213168_p(SourceFile:118) ~[?:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:computing_frames,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.server.MinecraftServer.func_213205_aW(MinecraftServer.java:717) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.server.MinecraftServer.func_213168_p(MinecraftServer.java:711) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.util.concurrent.ThreadTaskExecutor.func_213161_c(SourceFile:127) ~[?:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:computing_frames,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.server.MinecraftServer.func_213202_o(MinecraftServer.java:697) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.server.MinecraftServer.func_240802_v_(MinecraftServer.java:646) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.server.MinecraftServer.func_240783_a_(MinecraftServer.java:232) ~[?:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:byg.mixins.json:server.MixinMinecraftServer,pl:mixin:A,pl:runtimedistcleaner:A}
	at java.lang.Thread.run(Thread.java:748) [?:1.8.0_292] {}


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
Details:
	Minecraft Version: 1.16.5
	Minecraft Version ID: 1.16.5
	Operating System: Linux (amd64) version 4.18.0-372.9.1.el8.x86_64
	Java Version: 1.8.0_292, AdoptOpenJDK
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), AdoptOpenJDK
	Memory: 758802536 bytes (723 MB) / 3317694464 bytes (3164 MB) up to 6524764160 bytes (6222 MB)
	CPUs: 3
	JVM Flags: 2 total; -Xmx7000M -Xms128M
	ModLauncher: 8.1.3+8.1.3+main-8.1.x.c94d18ec
	ModLauncher launch target: fmlserver
	ModLauncher naming: srg
	ModLauncher services: 
		/mixin-0.8.4.jar mixin PLUGINSERVICE 
		/eventbus-4.0.0.jar eventbus PLUGINSERVICE 
		/forge-1.16.5-36.2.34.jar object_holder_definalize PLUGINSERVICE 
		/forge-1.16.5-36.2.34.jar runtime_enum_extender PLUGINSERVICE 
		/accesstransformers-3.0.1.jar accesstransformer PLUGINSERVICE 
		/forge-1.16.5-36.2.34.jar capability_inject_definalize PLUGINSERVICE 
		/forge-1.16.5-36.2.34.jar runtimedistcleaner PLUGINSERVICE 
		/mixin-0.8.4.jar mixin TRANSFORMATIONSERVICE 
		/OptiFine_1.16.5_HD_U_G8%20(1).jar OptiFine TRANSFORMATIONSERVICE 
		/forge-1.16.5-36.2.34.jar fml TRANSFORMATIONSERVICE 
	FML: 36.2
	Forge: net.minecraftforge:36.2.34
	FML Language Providers: 
		javafml@36.2
		minecraft@1
	Mod List: 
		forge-1.16.5-36.2.34-server.jar                   |Minecraft                     |minecraft                     |1.16.5              |DONE      |Manifest: NOSIGNATURE
		BrassAmberBattleTowers-1.16.5-1.6.3.jar           |Brass Amber BattleTowers      |ba_bt                         |1.16.5-1.6.3        |DONE      |Manifest: NOSIGNATURE
		SkyVillage_1.0.0_1.16.5.jar                       |Sky Villages                  |skyvillages                   |1.0.0               |DONE      |Manifest: NOSIGNATURE
		repurposed_structures_forge-3.4.7+1.16.5.jar      |Repurposed Structures         |repurposed_structures         |3.4.7+1.16.5        |DONE      |Manifest: NOSIGNATURE
		morevillagers-FORGE-1.16.5-1.5.5.jar              |More Villagers                |morevillagers                 |1.5.5               |DONE      |Manifest: NOSIGNATURE
		DungeonsMod-1.16.3-1.4.43.jar                     |Dungeons Mod                  |dungeonsmod                   |1.16.3-1.4.43       |DONE      |Manifest: NOSIGNATURE
		MouseTweaks-2.14-mc1.16.2.jar                     |Mouse Tweaks                  |mousetweaks                   |2.14                |DONE      |Manifest: NOSIGNATURE
		TrashSlot_1.16.3-12.2.1.jar                       |TrashSlot                     |trashslot                     |12.2.1              |DONE      |Manifest: NOSIGNATURE
		infernal-expansion-1.16.5-2.5.0.jar               |Infernal Expansion            |infernalexp                   |2.5.0               |DONE      |Manifest: NOSIGNATURE
		jei-1.16.5-7.7.1.152.jar                          |Just Enough Items             |jei                           |7.7.1.152           |DONE      |Manifest: NOSIGNATURE
		abnormals_core-1.16.5-3.3.1.jar                   |Abnormals Core                |abnormals_core                |3.3.1               |DONE      |Manifest: NOSIGNATURE
		LibraryFerret-Forge-1.16.5-2.0.0.jar              |Library ferret                |libraryferret                 |2.0.0               |DONE      |Manifest: NOSIGNATURE
		SpartanShields-1.16.5-2.1.2.jar                   |Spartan Shields               |spartanshields                |2.1.2               |DONE      |Manifest: NOSIGNATURE
		BetterCaves-Forge-1.16.4-1.1.2.jar                |YUNG's Better Caves           |bettercaves                   |1.16.4-1.1.2        |DONE      |Manifest: NOSIGNATURE
		villagernames_1.16.5-3.4.jar                      |Villager Names                |villagernames                 |3.4                 |DONE      |Manifest: NOSIGNATURE
		collective-1.16.5-4.28.jar                        |Collective                    |collective                    |4.28                |DONE      |Manifest: NOSIGNATURE
		Clumps-6.0.0.28.jar                               |Clumps                        |clumps                        |6.0.0.28            |DONE      |Manifest: NOSIGNATURE
		journeymap-1.16.5-5.7.3.jar                       |Journeymap                    |journeymap                    |5.7.3               |DONE      |Manifest: NOSIGNATURE
		citadel-1.8.1-1.16.5.jar                          |Citadel                       |citadel                       |1.8.1               |DONE      |Manifest: NOSIGNATURE
		alexsmobs-1.12.1.jar                              |Alex's Mobs                   |alexsmobs                     |1.12.1              |DONE      |Manifest: NOSIGNATURE
		AutoRegLib-1.6-49.jar                             |AutoRegLib                    |autoreglib                    |1.6-49              |DONE      |Manifest: NOSIGNATURE
		StorageDrawers-1.16.3-8.5.2.jar                   |Storage Drawers               |storagedrawers                |8.5.2               |DONE      |Manifest: NOSIGNATURE
		YungsExtras-Forge-1.16.4-1.0.jar                  |YUNG's Extras                 |yungsextras                   |Forge-1.16.4-1.0    |DONE      |Manifest: NOSIGNATURE
		jumpboat-1.16.5-0.1.0.2.jar                       |Jumpy Boats                   |jumpboat                      |1.16.5-0.1.0.2      |DONE      |Manifest: NOSIGNATURE
		YungsApi-1.16.4-Forge-13.jar                      |YUNG's API                    |yungsapi                      |1.16.4-Forge-13     |DONE      |Manifest: NOSIGNATURE
		BetterVillage-Forge-1.16.5-1.0.2.jar              |Better Village                |bettervillage                 |1                   |DONE      |Manifest: NOSIGNATURE
		stoneholm-1.2.2.jar                               |Stoneholm                     |stoneholm                     |1.2                 |DONE      |Manifest: NOSIGNATURE
		OuterEnd-0.2.14.jar                               |The Outer End                 |outer_end                     |0.2.9               |DONE      |Manifest: NOSIGNATURE
		tombstone-6.7.8-1.16.5.jar                        |Corail Tombstone              |tombstone                     |6.7.8               |DONE      |Manifest: NOSIGNATURE
		BetterStrongholds-1.16.4-1.2.1.jar                |YUNG's Better Strongholds     |betterstrongholds             |1.16.4-1.2.1        |DONE      |Manifest: NOSIGNATURE
		Bookshelf-Forge-1.16.5-10.4.32.jar                |Bookshelf                     |bookshelf                     |10.4.32             |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		EnchantmentDescriptions-1.16.5-7.0.18.jar         |EnchantmentDescriptions       |enchdesc                      |7.0.18              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		SpartanWeaponry-1.16.5-2.2.0-rc-2.jar             |Spartan Weaponry              |spartanweaponry               |2.2.0 Release Candid|DONE      |Manifest: NOSIGNATURE
		mcw-furniture-3.0.0-mc1.16.5.jar                  |Macaw's Furniture             |mcwfurnitures                 |3.0.0               |DONE      |Manifest: NOSIGNATURE
		Hwyla-forge-1.10.11-B78_1.16.2.jar                |Waila                         |waila                         |1.10.11-B78_1.16.2  |DONE      |Manifest: NOSIGNATURE
		cloth-config-4.14.64-forge.jar                    |Cloth Config v4 API           |cloth-config                  |4.14.64             |DONE      |Manifest: NOSIGNATURE
		byg-1.3.5.jar                                     |Oh The Biomes You'll Go       |byg                           |1.3.4               |DONE      |Manifest: NOSIGNATURE
		forge-1.16.5-36.2.34-universal.jar                |Forge                         |forge                         |36.2.34             |DONE      |Manifest: 22:af:21:d8:19:82:7f:93:94:fe:2b:ac:b7:e4:41:57:68:39:87:b1:a7:5c:c6:44:f9:25:74:21:14:f5:0d:90
		Quark-r2.4-322.jar                                |Quark                         |quark                         |r2.4-322            |DONE      |Manifest: NOSIGNATURE
		endergetic-1.16.5-3.0.2.jar                       |The Endergetic Expansion      |endergetic                    |3.0.2               |DONE      |Manifest: NOSIGNATURE
		appleskin-forge-mc1.16.x-2.4.0.jar                |AppleSkin                     |appleskin                     |2.4.0+mc1.16.4      |DONE      |Manifest: NOSIGNATURE
		valhelsia_core-16.0.15.jar                        |Valhelsia Core                |valhelsia_core                |16.0.15             |DONE      |Manifest: NOSIGNATURE
		valhelsia_structures-1.16.5-0.1.6.jar             |Valhelsia Structures          |valhelsia_structures          |1.16.5-0.1.6        |DONE      |Manifest: NOSIGNATURE
		supplementaries-1.16.5-0.18.4.jar                 |Supplementaries               |supplementaries               |0.18.2              |DONE      |Manifest: NOSIGNATURE
		BetterMineshafts-Forge-1.16.4-2.0.4.jar           |YUNG's Better Mineshafts      |bettermineshafts              |1.16.4-2.0.4        |DONE      |Manifest: NOSIGNATURE
		selene-1.16.5-1.9.0.jar                           |Selene                        |selene                        |1.16.5-1.0          |DONE      |Manifest: NOSIGNATURE
		mcw-lights-1.0.3-mc1.16.5.jar                     |Macaw's Lights and Lamps      |mcwlights                     |1.0.3               |DONE      |Manifest: NOSIGNATURE
		DungeonsArise-1.16.5-2.1.49-beta.jar              |When Dungeons Arise           |dungeons_arise                |2.1.49              |DONE      |Manifest: NOSIGNATURE
	Crash Report UUID: 79465233-0812-400b-9f03-24bc19adea8d
	Player Count: 1 / 100; [ServerPlayerEntity['Gerlus'/19081, l='ServerLevel[world]', x=-249.17, y=69.00, z=119.87]]
	Data Packs: vanilla, mod:ba_bt, mod:skyvillages, mod:repurposed_structures, mod:morevillagers, mod:dungeonsmod (incompatible), mod:mousetweaks, mod:trashslot (incompatible), mod:infernalexp (incompatible), mod:jei, mod:abnormals_core, mod:libraryferret, mod:spartanshields, mod:bettercaves (incompatible), mod:villagernames, mod:collective, mod:clumps, mod:journeymap (incompatible), mod:citadel (incompatible), mod:alexsmobs, mod:autoreglib (incompatible), mod:storagedrawers (incompatible), mod:yungsextras, mod:jumpboat, mod:yungsapi, mod:bettervillage, mod:stoneholm, mod:outer_end, mod:tombstone, mod:betterstrongholds, mod:bookshelf, mod:enchdesc, mod:spartanweaponry, mod:mcwfurnitures, mod:waila, mod:cloth-config (incompatible), mod:byg, mod:forge, mod:quark (incompatible), mod:endergetic, mod:appleskin, mod:valhelsia_core, mod:valhelsia_structures, mod:supplementaries, mod:bettermineshafts, mod:selene, mod:mcwlights, mod:dungeons_arise
	Is Modded: Definitely; Server brand changed to 'forge'
	Type: Dedicated Server (map_server.txt)
