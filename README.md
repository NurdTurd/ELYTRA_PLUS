# ELYTRA_PLUS
Code for Elytra +:


package ElytraPlus;

import org.bukkit.Material;

import org.bukkit.inventory.ItemStack;

import org.bukkit.inventory.ShapedRecipe

import org.bukkit.plugin.java.JavaPlugin;


public class ElytraPlus extends JavaPlugin {

	public ElytraPlus() {
	
	}

	public void onEnable() {
	
		ItemStack itemstack = new ItemStack(Material.ELYTRA);
		
		ShapedRecipe recipe = new ShapedRecipe(itemstack);
		
		recipe.shape(new String[] {
		
				"WVW",
				
				"L L",
				
				"S S" }
				
		recipe.setIngredient('S', Material.STICK);
		
		recipe.setIngredient('L', Material.LEATHER);
		
		recipe.setIngredient('W', Material.WOOL);
		
		recipe.setIngredient('V', Material.FEATHER);
		
		getServer().addRecipe(recipe);
	}
}
