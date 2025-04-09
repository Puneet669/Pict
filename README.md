# Pict



@model Members

<h2>Create Member</h2>

@if (ViewBag.Message != null)
{
    <h2 id="Message">@ViewBag.Message</h2>
}

<form asp-action="CreateMembership" method="post">
    <div><label>Name</label><input asp-for="Name" /><span asp-validation-for="Name"></span></div>
    <div><label>Gender</label><input asp-for="Gender" /><span asp-validation-for="Gender"></span></div>
    <div><label>Contact</label><input asp-for="Contact" /><span asp-validation-for="Contact"></span></div>
    <div>
        <label>Branch</label>
        <select asp-for="BranchId" asp-items="Model.Branches"></select>
        <span asp-validation-for="BranchId"></span>
    </div>
    <button type="submit" id="MemberCreationBtn">Create</button>
</form>
