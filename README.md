Небольшое дополнение, добавляющее во FlashDevelop кнопку прибития всех процессов FlashPlayerDebugger.exe

Для установки скопируйте приложение flashkiller.exe в удобное для вас место, после чего добавьте допишите в файл 

	Путь\установки\FlashDevelop\Settings\ToolBar.xml

в секцию toolbar строку 

	<button label="Kill FlashPlayer" click="RunProcess" tag="Путь/до/flashkiller/flashkiller.exe" image="192" />

Пример моего ToolBar.xml

	<?xml version="1.0" encoding="utf-8" ?>
	<toolbar>
		<button label="Label.New" click="New" image="275" />
		<button label="Label.Open" click="Open" image="214" />
		<button label="Label.Save" click="Save" image="168" flags="Enable:IsEditable|IsModified" />
		<button label="Label.SaveAll" click="SaveAll" image="169" flags="Enable:HasModified" />
		<button label="Label.Print" click="Print" image="343" flags="Enable:IsEditable" />
		<separator />
		<button label="Label.ToggleBookmark" click="ToggleBookmark" image="402" flags="Enable:IsEditable" />
		<button label="Label.NextBookmark" click="NextBookmark" image="402|9|3|3" flags="Enable:IsEditable" />
		<button label="Label.PrevBookmark" click="PrevBookmark" image="402|1|-3|3" flags="Enable:IsEditable" />
		<button label="Label.ClearBookmarks" click="ClearBookmarks" image="402|4|4|4" flags="Enable:IsEditable" />
		<separator />
		<button label="Label.CommandPrompt" click="PluginCommand" tag="FileExplorer.PromptHere;$(ProjectDir)" image="57" />
		<button label="Label.WindowsExplorer" click="PluginCommand" tag="FileExplorer.Explore;$(ProjectDir)" image="46" />
		<button label="Label.CodeSnippets" click="EditSnippets" image="341|5|2|2" />

		<button label="Kill FlashPlayer" click="RunProcess" tag="C:/Program Files (x86)/FlashDevelop/Tools/flashkiller.exe" image="192" />
	</toolbar>


