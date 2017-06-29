# hello-world
crash codes
---- Minecraft Crash Report ----

WARNING: coremods are present:
  CCLCorePlugin (CodeChickenLib-1.10.2-2.5.7.241-universal.jar)
  Brandon's Core (BrandonsCore-1.10.2-2.1.6.98-universal.jar)
  IvToolkit (IvToolkit-1.3.2.1-1.10.jar)
  EnderCorePlugin (EnderCore-1.10.2-0.4.1.65-beta.jar)
  NEICorePlugin (NotEnoughItems-1.10.2-2.1.3.207-universal.jar)
  PlusTiC (plustic-4.3.0.2.jar)
  MalisisCorePlugin (malisiscore-1.10.2-4.4.0.jar)
  LoadingPlugin (ResourceLoader-MC1.9.4-1.5.1.jar)
  FMLPlugin (InventoryTweaks-1.61-58.jar)
  ForgelinPlugin (Forgelin-1.4.1.jar)
  ChiselCorePlugin (Chisel-MC1.10.2-0.0.9.15.jar)
  CoFH Loading Plugin (CoFHCore-1.10.2-4.1.1.156-universal.jar)
Contact their authors BEFORE contacting forge

// Why did you do that?

Time: 6/29/17 5:05 PM
Description: There was a severe problem during mod loading that has caused the game to fail

net.minecraftforge.fml.common.LoaderExceptionModCrash: Caught exception from CoFH Core (cofhcore)
Caused by: java.lang.NoClassDefFoundError: com/typesafe/config/ConfigException
	at cofh.CoFHCore.registerHandlers(CoFHCore.java:138)
	at cofh.CoFHCore.preInit(CoFHCore.java:78)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:483)
	at net.minecraftforge.fml.common.FMLModContainer.handleModStateEvent(FMLModContainer.java:616)
	at sun.reflect.GeneratedMethodAccessor2.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:483)
	at com.google.common.eventbus.EventSubscriber.handleEvent(EventSubscriber.java:74)
	at com.google.common.eventbus.SynchronizedEventSubscriber.handleEvent(SynchronizedEventSubscriber.java:47)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:322)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:304)
	at com.google.common.eventbus.EventBus.post(EventBus.java:275)
	at net.minecraftforge.fml.common.LoadController.sendEventToModContainer(LoadController.java:243)
	at net.minecraftforge.fml.common.LoadController.propogateStateMessage(LoadController.java:221)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:483)
	at com.google.common.eventbus.EventSubscriber.handleEvent(EventSubscriber.java:74)
	at com.google.common.eventbus.SynchronizedEventSubscriber.handleEvent(SynchronizedEventSubscriber.java:47)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:322)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:304)
	at com.google.common.eventbus.EventBus.post(EventBus.java:275)
	at net.minecraftforge.fml.common.LoadController.distributeStateMessage(LoadController.java:145)
	at net.minecraftforge.fml.common.Loader.preinitializeMods(Loader.java:624)
	at net.minecraftforge.fml.client.FMLClientHandler.beginMinecraftLoading(FMLClientHandler.java:259)
	at net.minecraft.client.Minecraft.func_71384_a(Minecraft.java:439)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:351)
	at net.minecraft.client.main.Main.main(SourceFile:124)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:483)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)
Caused by: java.lang.ClassNotFoundException: com.typesafe.config.ConfigException
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:191)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:424)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:357)
	... 38 more
Caused by: java.lang.NullPointerException
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:182)
	... 40 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
Details:
	Minecraft Version: 1.10.2
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_25, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 2278261552 bytes (2172 MB) / 3692560384 bytes (3521 MB) up to 6681526272 bytes (6372 MB)
	JVM Flags: 4 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx7168m -Xms256m -XX:PermSize=256m
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP 9.32 Powered by Forge 12.18.3.2281 135 mods loaded, 135 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCH	mcp{9.19} [Minecraft Coder Pack] (minecraft.jar) 
	UCH	FML{8.0.99.99} [Forge Mod Loader] (forge-1.10.2-12.18.3.2281.jar) 
	UCH	Forge{12.18.3.2281} [Minecraft Forge] (forge-1.10.2-12.18.3.2281.jar) 
	UCH	ivtoolkit{1.3.2.1-1.10} [IvToolkit] (minecraft.jar) 
	UCH	NotEnoughItems{2.1.3.207} [Not Enough Items] (NotEnoughItems-1.10.2-2.1.3.207-universal.jar) 
	UCH	<CoFH ASM>{000} [CoFH ASM] (minecraft.jar) 
	UCH	ccl-entityhook{1.0} [ccl-entityhook] (CodeChickenLib-1.10.2-2.5.7.241-universal.jar) 
	UCH	infinitylib{1.10.2-0.8.0} [InfinityLib] (infinitylib-0.8.0.jar) 
	UCH	agricraft{2.0.0-0.8.0-a15} [AgriCraft] (agricraft-2.0.0-0.8.0-a15.jar) 
	UCH	Baubles{1.3.9} [Baubles] (Baubles-1.10.2-1.3.9.jar) 
	UCH	JEI{3.14.7.417} [Just Enough Items] (jei_1.10.2-3.14.7.417.jar) 
	UCE	cofhcore{4.1.1} [CoFH Core] (CoFHCore-1.10.2-4.1.1.156-universal.jar) 
	UCH	extrautils2{1.0} [Extra Utilities 2] (extrautils2-1.10.2-1.4.jar) 
	UCH	flyringbaublemod{0.2.3_1.10.2-d3100bf} [AngelRing 2 Bauble] (angelRingToBauble-1.10.2-0.2.3.16+d3100bf.jar) 
	UCH	appleskin{1.0.5} [AppleSkin] (AppleSkin-mc1.10.2-1.0.5.jar) 
	UCH	architecturecraft{1.7.1} [ArchitectureCraft] (ArchitectureCraft-1.7.1-mc1.10.2.jar) 
	UCH	Avaritia{1.10.2-2.0.7} [Avaritia] (Avaritia-1.10.2-2.0.7.jar) 
	UCH	avaritiaadditions{1.6} [Avaritia Additions] (AvaritiaAdditions-1.6_1.10.2.jar) 
	UCH	baconators{3.0.5} [Baconators] (baconators-1.10.2-3.0.5.jar) 
	UCH	crafttweakerjei{1.0.1} [CraftTweaker JEI Support] (CraftTweaker-1.10.2-3.0.24.jar) 
	UCH	MineTweaker3{3.0.24} [MineTweaker 3] (CraftTweaker-1.10.2-3.0.24.jar) 
	UCH	base{1.10.2-1.3.0} [B.A.S.E] (base-1.10.2-1.3.0.jar) 
	UCH	betterbuilderswands{0.11.1} [Better Builder's Wands] (BetterBuildersWands-1.10.2-0.11.1.220+f8232fe.jar) 
	UCH	BiomesOPlenty{5.0.0.2162} [Biomes O' Plenty] (BiomesOPlenty-1.10.2-5.0.0.2162-universal.jar) 
	UCH	blockarmor{2.4.3} [Block Armor] (BlockArmor-1.10.2-2.4.3.jar) 
	UCH	Botania{r1.9-341} [Botania] (Botania r1.9-341.jar) 
	UCH	CodeChickenLib{2.5.7.241} [CodeChicken Lib] (CodeChickenLib-1.10.2-2.5.7.241-universal.jar) 
	UCH	brandonscore{2.1.6} [Brandon's Core] (BrandonsCore-1.10.2-2.1.6.98-universal.jar) 
	UCH	Chameleon{1.10-2.2.2} [Chameleon] (Chameleon-1.10-2.2.2.jar) 
	UCH	chancecubes{1.10.2-2.3.5.174} [Chance Cubes] (ChanceCubes-1.10.2-2.3.5.174.jar) 
	UCH	ChestTransporter{2.5.13} [Chest Transporter] (ChestTransporter-1.10.2-2.5.13.jar) 
	UCH	CodeChickenCore{2.4.1.102} [CodeChicken Core] (CodeChickenCore-1.10.2-2.4.1.102-universal.jar) 
	UCH	ChickenChunks{2.2.0.52} [ChickenChunks] (ChickenChunks-1.10.2-2.2.0.52-universal.jar) 
	UCH	chickens{4.3.2} [Chickens] (chickens-4.3.2.jar) 
	UCH	chisel{MC1.10.2-0.0.9.15} [Chisel] (Chisel-MC1.10.2-0.0.9.15.jar) 
	UCH	mcmultipart{1.4.0} [MCMultiPart] (MCMultiPart-1.4.0-universal.jar) 
	UCH	chiselsandbits{12.12} [Chisels & Bits] (chiselsandbits-12.12.jar) 
	UCH	clumps{1.0.5} [Clumps] (Clumps-1.0.5.jar) 
	UCH	cyclopscore{0.10.0} [Cyclops Core] (CyclopsCore-1.9.4-0.10.0.jar) 
	UCH	colossalchests{1.5.0} [Colossal Chests] (ColossalChests-1.10.2-1.5.0.jar) 
	UCH	one_point_twelve_concrete{4.1 APRIL FOOLS} [1.12 Concrete] (concreteMod-4.1-APRILFOOLS.jar) 
	UCH	cookingforblockheads{4.2.39} [Cooking for Blockheads] (CookingForBlockheads_1.10.2-4.2.39.jar) 
	UCH	craftingtweaks{6.1.16} [Crafting Tweaks] (CraftingTweaks_1.10.2-6.1.16.jar) 
	UCH	ctgui{1.0.0} [CT-GUI] (CraftTweaker-1.10.2-3.0.24.jar) 
	UCH	cropdusting{0.6} [CropDusting] (CropDusting-0.6-[1.9.4-1.10-1.10.2].jar) 
	UCH	modcurrency{1.10.2-1.0.3} [Currency Mod] (Currency-1.10.2-1.0.3.jar) 
	UCH	CustomMainMenu{2.0.2} [Custom Main Menu] (CustomMainMenu-MC1.10.2-2.0.2.jar) 
	UCH	PTRModelLib{1.0.0} [PTRModelLib] (Decocraft-2.4.1_1.10.2.jar) 
	UCH	props{2.4.1} [Decocraft] (Decocraft-2.4.1_1.10.2.jar) 
	UCH	draconicevolution{2.0.10} [Draconic Evolution] (Draconic-Evolution-1.10.2-2.0.10.199-universal.jar) 
	UCH	elevatorid{1.3.0} [Elevator Mod] (ElevatorMod[V.1.3.0][MC.1.10.2].jar) 
	UCH	endercore{1.10.2-0.4.1.65-beta} [EnderCore] (EnderCore-1.10.2-0.4.1.65-beta.jar) 
	UCH	Waila{1.8.13-B27_1.10.2} [Waila] (Hwyla-1.8.13-B27_1.10.2.jar) 
	UCH	EnderIO{1.10.2-3.1.180} [Ender IO] (EnderIO-1.10.2-3.1.180.jar) 
	UCH	EnderStorage{2.2.1.106} [EnderStorage] (EnderStorage-1.10.2-2.2.1.106-universal.jar) 
	UCH	EnderZoo{1.10-1.2.3.44} [Ender Zoo] (EnderZoo-1.10-1.2.3.44.jar) 
	UCH	fakeblocks{1.0.0} [FakeBlocks] (FakeBlocks 1.0.0.jar) 
	UCH	FastLeaveDecay{1.2.3} [Fast Leave Decay] (FastLeaveDecay-MC1.10.2-1.2.3.jar) 
	UCH	flatcoloredblocks{mc1.10-v4.4} [Flat Colored Blocks] (flatcoloredblocks-mc1.10-v4.4.jar) 
	UCH	foamfix{@VERSION@} [FoamFix] (foamfix-0.6.1-law.jar) 
	UCH	forgelin{1.4.1} [Forgelin] (Forgelin-1.4.1.jar) 
	UCH	ftbl{0.0.0} [FTBLib] (FTBLib-1.1x-3.5.4.jar) 
	UCH	ftbu{0.0.0} [FTBUtilities] (FTBUtilities-1.1x-3.5.4.jar) 
	UCH	googlyeyes{6.0.0} [GooglyEyes] (GooglyEyes-1.10.2-6.0.0.jar) 
	UCH	gravestone{1.5.12} [Gravestone] (GraveStone Mod 1.5.12.jar) 
	UCH	hatchery{0.2.10} [Hatchery] (hatchery-1.10.2-0.2.10.jar) 
	UCH	hermitron{0.2.12} [Hermitron] (hermitron-1.10.2-0.2.12.jar) 
	UCH	ichunutil{6.3.0} [iChunUtil] (iChunUtil-1.10.2-6.3.0.jar) 
	UCH	InventoryPets{1.4.9.3} [Inventory Pets] (inventorypets-1.10-1.4.9.3.jar) 
	UCH	inventorytweaks{1.61-58-a1fd884} [Inventory Tweaks] (InventoryTweaks-1.61-58.jar) 
	UCH	ironchest{1.10.2-7.0.11.797} [Iron Chest] (ironchest-1.10.2-7.0.11.797.jar) 
	UCH	iskalliumreactors{0.3.8-beta} [Iskallium Reactors] (iskalliumreactors-1.10.2-0.3.8-beta.jar) 
	UCH	journeymap{1.10.2-5.4.6} [JourneyMap] (journeymap-1.10.2-5.4.6.jar) 
	UCH	loottweaker{0.0.5.1} [LootTweaker] (LootTweaker-1.10.2-0.0.5.1.jar) 
	UCH	jeresources{0.5.8.98} [Just Enough Resources] (JustEnoughResources-1.10.2-0.5.8.98.jar) 
	UCH	librarianlib{1.10.1} [LibrarianLib] (librarianlib-1.10.1.jar) 
	UCH	lootbags{2.3.7} [Loot Bags] (LootBags-1.10.2-2.3.7.jar) 
	UCH	malisiscore{1.10.2-4.4.0} [MalisisCore] (malisiscore-1.10.2-4.4.0.jar) 
	UCH	malisisdoors{1.10.2-5.2.0} [MalisisDoors] (malisisdoors-1.10.2-5.2.0.jar) 
	UCH	mantle{1.10.2-1.1.5.205} [Mantle] (Mantle-1.10.2-1.1.5.jar) 
	UCH	RadixCore{1.10.2-2.1.3} [RadixCore] (RadixCore-1.10.2-2.1.3-universal.jar) 
	UCH	MCA{1.10.2-5.2.3} [Minecraft Comes Alive] (MCA-1.10.2-5.2.3-universal.jar) 
	UCH	mtrm{1.2.1.26} [MineTweakerRecipeMaker] (MineTweakerRecipeMaker-1.10.2-1.2.1.26.jar) 
	UCH	natura{1.10.2-4.1.0.48} [Natura] (natura-1.10.2-4.1.0.48.jar) 
	UCH	railcraft{10.0.1} [Railcraft] (Railcraft_1.10.2-10.0.1.jar) 
	UCH	tconstruct{1.10.2-2.6.3.500} [Tinkers' Construct] (TConstruct-1.10.2-2.6.3.jar) 
	UCH	moarsigns{4.2.2.8} [MoarSigns] (MoarSigns-1.10.2-4.2.2.8.jar) 
	UCH	mobdismemberment{6.0.0} [MobDismemberment] (MobDismemberment-1.10.2-6.0.0.jar) 
	UCH	mob_grinding_utils{0.1.8.17} [mob_grinding_utils] (MobGrindingUtils-0.1.8.17.jar) 
	UCH	mtlib{@VERSION@} [MTLib] (MTLib-1.0.2.jar) 
	UCH	modtweaker{2.0.11} [Mod Tweaker] (ModTweaker2-2.0.11.jar) 
	UCH	morechickens{1.0.11} [More Chickens] (MoreChickens-1.10.2-1.0.11.jar) 
	UCH	moreloottables{0.2.1} [More Loot Tables] (moreloottables-1.10.2-0.2.1.jar) 
	UCH	moreplayermodels{1.10.2} [MorePlayerModels] (MorePlayerModels_1.10.2(11nov16).jar) 
	UCH	Morpheus{1.10.2-3.1.13} [Morpheus] (Morpheus-1.10.2-3.1.13.jar) 
	UCH	mousetweaks{2.8} [Mouse Tweaks] (MouseTweaks-2.8-mc1.10.2.jar) 
	UCH	mw{1.9.1} [Modern Warfare] (mw-1.9.1_mc1.10.2.jar) 
	UCH	mysticalagriculture{1.5.1} [Mystical Agriculture] (mysticalagriculture[1.10.2]-1.5.1.jar) 
	UCH	botanicaladdons{1.9} [Natural Pledge] (NaturalPledge-r1.9.1.jar) 
	UCH	nethercore{1.10.2-2.0.3} [Nether Core] (nethercore-1.10.2-2.0.3.jar) 
	UCH	recipehandler{0.6} [NoMoreRecipeConflict] (NoMoreRecipeConflict-0.6(1.10.2).jar) 
	UCH	harvestcraft{1.9.4-1.10.2g} [Pam's HarvestCraft] (Pam's HarvestCraft 1.9.4-1.10.2h.jar) 
	UCE	thermalfoundation{2.0.5} [Thermal Foundation] (ThermalFoundation-1.10.2-2.0.5.81-universal.jar) 
	UCE	plustic{4.3.0.2} [PlusTiC] (plustic-4.3.0.2.jar) 
	UCH	progressiveautomation{1.7.4} [Progressive Automation] (ProgressiveAutomation-1.10.2-1.7.4.jar) 
	UCH	reccomplex{1.2.10-1.10} [Recurrent Complex] (RecurrentComplex-1.2.10-1.10.jar) 
	UCH	StorageDrawers{1.10.2-3.7.1} [Storage Drawers] (StorageDrawers-1.10.2-3.7.1.jar) 
	UCH	refinedstorage{1.2.25} [Refined Storage] (refinedstorage-1.2.25.jar) 
	UCH	ResourceLoader{1.5.1} [Resource Loader] (ResourceLoader-MC1.9.4-1.5.1.jar) 
	UCH	rftools{5.92} [RFTools] (rftools-1.1x-5.92.jar) 
	UCH	roguelike{1.5.9} [Roguelike Dungeons] (RoguelikeDungeons-1.10.2-1.5.9.jar) 
	UCH	shadowmc{3.6.1} [ShadowMC] (ShadowMC-1.10.2-3.6.1.jar) 
	UCH	SimpleLabels{0.0.1} [SimpleLabels] (simplelabels-1-10.2-0.0.3.jar) 
	UCH	simplyconveyors{3.0.3} [Simply Conveyors & More] (SimplyConveyors-1.10.2-3.0.3.jar) 
	UCH	SleepingBag{1.4.0} [Sleeping Bag] (SleepingBag-1.10.2-1.4.0.jar) 
	UCH	subcommonlib{1.1.3.0} [Subaraki's Common Library] (sublib-1.10.2-1.1.3.0.jar) 
	UCE	thermalexpansion{5.0.4} [Thermal Expansion] (ThermalExpansion-1.10.2-5.0.4.90-universal.jar) 
	UCH	tinkertoolleveling{1.10.2-1.0.1.DEV.f5def58} [Tinkers Tool Leveling] (TinkerToolLeveling-1.10.2-1.0.1.jar) 
	UCH	tp{1.2.0-Hotfix} [Tiny Progressions] (tinyprogressions-1.10.2-1.2.0-Hotfix.jar) 
	UCH	torchmaster{1.0} [TorchMaster] (torchmaster_1.10.2-1.2.1.23.jar) 
	UCH	Translocator{2.1.4.55} [Translocator] (Translocators-1.10.2-2.1.4.55-universal.jar) 
	UCH	usefulnullifiers{1.3.4} [Useful Nullifiers] (usefulnullifiers-1.3.4.jar) 
	UCH	VeinMiner{0.35.3_1.9-a46c1b0} [Vein Miner] (VeinMiner-1.9-0.35.3.595+a46c1b0.jar) 
	UCH	VeinMinerModSupport{0.35.3_1.9-a46c1b0} [Mod Support] (VeinMiner-1.9-0.35.3.595+a46c1b0.jar) 
	UCH	vc{4.26.13} [ViesCraft] (ViesCraft-1.10.X-4.26.13.jar) 
	UCH	wailafeatures{0.3.1.13} [WAILA Features] (WAILA-features-1.10.2-0.3.1.13.jar) 
	UCH	WailaHarvestability{1.1.9} [Waila Harvestability] (WailaHarvestability-mc1.10.2-1.1.9.jar) 
	UCH	icse{1.1.0.0} [I Can See Everything] (Wawla-1.10.2-2.3.2.215.jar) 
	UCH	wawla{2.3.2.215} [What Are We Looking At] (Wawla-1.10.2-2.3.2.215.jar) 
	UCH	waystones{2.0.12} [Waystones] (Waystones_1.10.2-2.0.12.jar) 
	UCH	weaponcaseloot{4.0.3} [WeaponCaseLoot] (weaponcaseloot-1.10.2-4.0.3.jar) 
	UCH	Woot{1.10.2-1.3.1} [Woot] (woot-1.10.2-1.3.1.jar) 
	UCH	xpplus{1.0} [XP-Plus] (xpplus-1.02.jar) 
	UCH	librarianliblate{1.10.1} [LibrarianLib Stage 2] (librarianlib-1.10.1.jar) 
	UCH	moofluids{1.10.2-1.7.02.12b} [Moo Fluids] (MooFluids-1.10.2-1.7.02.12b.jar) 
	Loaded coremods (and transformers): 
CCLCorePlugin (CodeChickenLib-1.10.2-2.5.7.241-universal.jar)
  codechicken.lib.asm.ClassHeirachyManager
  codechicken.lib.asm.CCL_ASMTransformer
Brandon's Core (BrandonsCore-1.10.2-2.1.6.98-universal.jar)
  com.brandon3055.brandonscore.asm.ClassTransformer
IvToolkit (IvToolkit-1.3.2.1-1.10.jar)
  
EnderCorePlugin (EnderCore-1.10.2-0.4.1.65-beta.jar)
  com.enderio.core.common.transform.EnderCoreTransformer
NEICorePlugin (NotEnoughItems-1.10.2-2.1.3.207-universal.jar)
  codechicken.nei.asm.NEITransformer
PlusTiC (plustic-4.3.0.2.jar)
  landmaster.plustic.asm.Transform
MalisisCorePlugin (malisiscore-1.10.2-4.4.0.jar)
  net.malisis.core.util.chunkcollision.ChunkCollisionTransformer
  net.malisis.core.util.chunkblock.ChunkBlockTransformer
  net.malisis.core.renderer.transformer.MalisisRendererTransformer
  net.malisis.core.renderer.icon.asm.TextureMapTransformer
  net.malisis.core.util.clientnotif.ClientNotifTransformer
LoadingPlugin (ResourceLoader-MC1.9.4-1.5.1.jar)
  lumien.resourceloader.asm.ClassTransformer
FMLPlugin (InventoryTweaks-1.61-58.jar)
  invtweaks.forge.asm.ContainerTransformer
ForgelinPlugin (Forgelin-1.4.1.jar)
  
ChiselCorePlugin (Chisel-MC1.10.2-0.0.9.15.jar)
  team.chisel.common.asm.ChiselTransformer
CoFH Loading Plugin (CoFHCore-1.10.2-4.1.1.156-universal.jar)
  cofh.asm.CoFHClassTransformer
  cofh.asm.repack.codechicken.lib.asm.ClassHierarchyManager
	GL info: ' Vendor: 'ATI Technologies Inc.' Version: '4.5.13474 Compatibility Profile Context 22.19.162.4' Renderer: 'AMD Radeon R7 200 Series'
	Pulsar/natura loaded Pulses: 
		- NaturaCommons (Enabled/Forced)
		- NaturaOverworld (Enabled/Not Forced)
		- NaturaNether (Enabled/Not Forced)
		- NaturaDecorative (Enabled/Not Forced)
		- NaturaEntities (Enabled/Not Forced)
		- NaturaOredict (Enabled/Forced)
		- NaturaWorld (Enabled/Not Forced)
		- WailaIntegration (Enabled/Not Forced)

	Pulsar/tconstruct loaded Pulses: 
		- TinkerCommons (Enabled/Forced)
		- TinkerWorld (Enabled/Not Forced)
		- TinkerTools (Enabled/Not Forced)
		- TinkerHarvestTools (Enabled/Forced)
		- TinkerMeleeWeapons (Enabled/Forced)
		- TinkerRangedWeapons (Enabled/Forced)
		- TinkerModifiers (Enabled/Forced)
		- TinkerSmeltery (Enabled/Not Forced)
		- TinkerGadgets (Enabled/Not Forced)
		- TinkerOredict (Enabled/Forced)
		- TinkerIntegration (Enabled/Forced)
		- TinkerFluids (Enabled/Forced)
		- TinkerMaterials (Enabled/Forced)
		- TinkerModelRegister (Enabled/Forced)
		- chiselsandbitsIntegration (Enabled/Not Forced)
		- craftingtweaksIntegration (Enabled/Not Forced)
		- WailaIntegration (Enabled/Not Forced)

	NotEnoughItems Invalid Fingerprint Reports: 
	CodeChickenLib Invalid Fingerprint Reports: 
	CodeChickenCore Invalid Fingerprint Reports: 
	ChickenChunks Invalid Fingerprint Reports: 
	EnderIO: Found the following problem(s) with your installation (That does NOT mean that Ender IO caused the crash or was involved in it in any way. We add this information to help finding common problems, not as an invitation to post any crash you encounter to Ender IO's issue tracker. Always check the stack trace above to see which mod is most likely failing.):
                  * An unsupportted RF API is installed (1.7.10R1.3.1 from BrandonsCore-1.10.2-2.1.6.98-universal.jar).
                    Ender IO needs at least 1.4.0 and will NOT work with older versions.
                 This may (look up the meaning of 'may' in the dictionary if you're not sure what it means) have caused the error. Try reproducing the crash WITHOUT this/these mod(s) before reporting it.
	Detailed RF API diagnostics:
                  * RF API class 'EnergyStorage' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/EnergyStorage.class
                  * RF API class 'IEnergyConnection' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/IEnergyConnection.class
                  * RF API class 'IEnergyContainerItem' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/IEnergyContainerItem.class
                  * RF API class 'IEnergyHandler' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/IEnergyHandler.class
                  * RF API class 'IEnergyProvider' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/IEnergyProvider.class
                  * RF API class 'IEnergyReceiver' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/IEnergyReceiver.class
                  * RF API class 'IEnergyStorage' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/IEnergyStorage.class
                  * RF API class 'ItemEnergyContainer' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/ItemEnergyContainer.class
                  * RF API class 'TileEnergyHandler' is loaded from: jar:file:/C:/Users/Owner/Documents/Curse/Minecraft/Instances/FoolCraft/mods/BrandonsCore-1.10.2-2.1.6.98-universal.jar!/cofh/api/energy/TileEnergyHandler.class
	Detailed Tesla API diagnostics:
                  * Tesla API class 'Tesla' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.Tesla)
                  * Tesla API class 'TeslaCapabilities' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.capability.TeslaCapabilities)
                  * Tesla API class 'ITeslaConsumer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.ITeslaConsumer)
                  * Tesla API class 'ITeslaHolder' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.ITeslaHolder)
                  * Tesla API class 'ITeslaProducer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.ITeslaProducer)
                  * Tesla API class 'BaseTeslaContainer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.BaseTeslaContainer)
                  * Tesla API class 'BaseTeslaContainerProvider' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.BaseTeslaContainerProvider)
                  * Tesla API class 'InfiniteTeslaConsumer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaConsumer)
                  * Tesla API class 'InfiniteTeslaConsumerProvider' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaConsumerProvider)
                  * Tesla API class 'InfiniteTeslaProducer' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaProducer)
                  * Tesla API class 'InfiniteTeslaProducerProvider' could not be loaded (reason: java.lang.ClassNotFoundException: net.darkhax.tesla.api.implementation.InfiniteTeslaProducerProvider)

	!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
	!!!You are looking at the diagnostics information, not at the crash. Scroll up!!!
	!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

	EnderStorage Invalid Fingerprint Reports: 
	Translocator Invalid Fingerprint Reports: 
