# Role-Control-System
The Role Control System is an advanced Discord bot extension that provides a comprehensive, user-friendly interface for managing server roles and permissions. It replaces Discord's clunky default role management with an intuitive control panel featuring interactive buttons, dropdown menus, and organized permission categories.
> 💡 **Built for the Zygnal Ecosystem — to download and use this extension, you must be part of the Zygnal Ecosystem.**  
> This extension (cog) is part of the **Zygnal Ecosystem** and is only available through its supported platforms.  
> You can use it with:  
> - The **[Discord Bot Framework](https://github.com/TheHolyOneZ/discord-bot-framework)** — ideal for developers who want full control and flexibility *(includes an integrated extension marketplace)*, or  
> - The **[ZygnalBot](https://zygnalbot.de)** — a prebuilt, plug-and-play Discord bot *(also includes an integrated extension marketplace)*.  
>
> Browse and install extensions at [zygnalbot.com/extension](https://zygnalbot.com/extension).  
> For help or community discussions, join us on Discord: [discord.gg/sgZnXca5ts](https://discord.gg/sgZnXca5ts)
# 🎛️ Role Control System Documentation

## 📋 Overview

The **Role Control System** is an advanced Discord bot extension that provides a comprehensive, user-friendly interface for managing server roles and permissions. It replaces Discord's clunky default role management with an intuitive control panel featuring interactive buttons, dropdown menus, and organized permission categories.

---

## 🚀 Getting Started

### 📝 Available Commands

| Command | Aliases | Description |
|---------|---------|-------------|
| **Main Panel** | `!rolecontrol` | `!rc`, `!rcontrol` | Open the interactive role control panel |
| **Panel Access** | `!rolecontrol panel` | `!rc main`, `!rc menu` | Alternative way to open the main panel |
| **Quick Create** | `!rolecontrol create <name>` | `!rc create <name>` | Instantly create a new role with default settings |
| **Edit Role** | `!rolecontrol edit <role>` | `!rc edit <role>` | Open management interface for existing role |
| **List Roles** | `!rolecontrol list` | `!rc list` | Display all server roles with statistics |
| **Role Info** | `!rolecontrol info <role>` | `!rc info <role>` | Show detailed information about a specific role |
| **Find Unused** | `!rolecontrol cleanup` | `!rc cleanup` | Identify roles with no members |
| **View Templates** | `!rolecontrol templates` | `!rc templates` | Display available role templates |
| **Help Guide** | `!rolecontrol help` | `!rc help` | Complete command reference and usage guide |

---

## 🎯 Core Features

### 🎛️ **Interactive Control Panel**
- **Beautiful Main Interface**: Clean, organized display with server statistics
- **Role Selection Dropdown**: Choose from existing roles or create new ones
- **Real-time Updates**: All changes reflect immediately in the interface
- **Visual Indicators**: Color-coded buttons and status displays

### ➕ **Role Creation & Management**
- **Quick Role Creation**: Create roles instantly with name and color
- **Appearance Editor**: Modify role names, colors, and display settings
- **Position Management**: Adjust role hierarchy and ordering
- **Bulk Operations**: Manage multiple roles efficiently

### 🔐 **Advanced Permission System**
The permission system is organized into **5 logical categories** for easy management:

#### ⚙️ **General Permissions**
- **Administrator** - Full server control (use with caution!)
- **Manage Server** - Server settings and configuration
- **Manage Roles** - Create and edit other roles
- **Manage Channels** - Create, edit, and delete channels
- **View Audit Log** - Access server audit history

#### 👥 **Membership Permissions**
- **Kick Members** - Remove members temporarily
- **Ban Members** - Permanently ban members
- **Create Invite** - Generate server invite links
- **Change Nickname** - Modify own display name
- **Manage Nicknames** - Change other members' nicknames

#### 💬 **Text Permissions**
- **Send Messages** - Post messages in text channels
- **Manage Messages** - Delete and edit others' messages
- **Embed Links** - Post rich link previews
- **Attach Files** - Upload images, documents, etc.
- **Mention Everyone** - Use @everyone and @here mentions

#### 🔊 **Voice Permissions**
- **Connect** - Join voice channels
- **Speak** - Talk in voice channels
- **Mute Members** - Mute others in voice
- **Deafen Members** - Deafen others in voice
- **Move Members** - Move users between voice channels

#### 🔧 **Advanced Permissions**
- **Manage Webhooks** - Create and manage webhooks
- **Manage Emojis** - Add, edit, and delete server emojis
- **Use App Commands** - Access slash commands and apps
- **Priority Speaker** - Override voice channel user limit
- **Video/Stream** - Share screen and camera in voice

### 📋 **Role Templates**
Pre-configured role setups for common server roles:

#### 🎯 **Moderator Template**
- **Purpose**: Full moderation capabilities
- **Permissions**: Kick, ban, manage messages, voice moderation
- **Color**: Red (#ff6b6b)
- **Settings**: Hoisted, mentionable

#### 🛠️ **Helper Template**
- **Purpose**: Basic moderation assistance
- **Permissions**: Manage messages, voice mute/deafen
- **Color**: Teal (#4ecdc4)
- **Settings**: Hoisted, mentionable

#### 👤 **Member Template**
- **Purpose**: Standard user permissions
- **Permissions**: Send messages, connect to voice, basic interactions
- **Color**: Blue (#45b7d1)
- **Settings**: Not hoisted, not mentionable

---

## 🛠️ How to Use

### 🎯 **Opening the Control Panel**
1. Type `!rolecontrol` in any channel
2. The main panel will appear with server statistics
3. Use the dropdown menu to select a role or create a new one

### ➕ **Creating a New Role**
1. Select "Create New Role" from the dropdown
2. Enter the role name and optional hex color
3. The role is created and management interface opens automatically

### ✏️ **Editing an Existing Role**
1. Select the role from the dropdown menu
2. Choose from available management options:
   - **Edit Permissions** - Modify role permissions by category
   - **Edit Appearance** - Change name, color, and display settings
   - **Role Position** - Adjust hierarchy and mentionable settings
   - **Apply Template** - Use pre-made configurations
   - **Delete Role** - Remove role permanently (with confirmation)

### 🔐 **Managing Permissions**
1. Click "Edit Permissions" on any role
2. Select a permission category (General, Membership, Text, Voice, Advanced)
3. Toggle individual permissions with colored buttons:
   - **🟢 Green** = Permission enabled
   - **⚫ Gray** = Permission disabled
4. Changes apply instantly when buttons are clicked

### 📋 **Using Templates**
1. Click "Apply Template" on any role
2. Select from available templates
3. All template settings (permissions, color, display) apply automatically
4. Templates can be customized by editing the JSON configuration files

---

## 🔒 Security & Safety Features

### ⚠️ **Permission Checks**
- Users can only edit roles **below** their highest role
- Server owners have unrestricted access
- Bot requires "Manage Roles" permission to function

### 🛡️ **Safety Measures**
- **Confirmation Dialogs** - Prevents accidental role deletion
- **Audit Logging** - All changes include proper reason tracking
- **Error Handling** - Graceful error messages for all operations
- **Role Hierarchy Respect** - Cannot edit roles above bot's position

### 📊 **Monitoring Features**
- **Real-time Statistics** - Live member counts and role usage
- **Change Logging** - Console logs for all role modifications
- **Unused Role Detection** - Identify roles with no members
- **Permission Warnings** - Highlights dangerous permissions

---

## 💡 Tips & Best Practices

### 🎯 **Role Organization**
- Use **templates** for consistent role setups
- Keep role **hierarchy** organized (higher = more permissions)
- Use **colors** to visually categorize roles
- Enable **hoist** for important roles to separate them in member lists

### 🔐 **Permission Management**
- Start with **minimal permissions** and add as needed
- Be **cautious** with Administrator permission (gives full access)
- Use **role hierarchy** instead of individual permissions when possible
- Regularly **audit** role permissions using the cleanup feature

### 🛠️ **Maintenance**
- Use `!rc cleanup` to find unused roles
- Review role **member counts** regularly
- Check **permission conflicts** between multiple roles
- Keep **templates updated** for new server needs

---

## 🆘 Troubleshooting

### ❌ **Common Issues**

**"Missing Manage Roles permission"**
- Ensure the bot has "Manage Roles" permission in server settings

**"Cannot edit this role"**
- Role may be higher than your highest role or the bot's role

**"Permission update failed"**
- Check if the bot's role is high enough in the hierarchy

**"Template not applying"**
- Verify template files exist in the RoleControl directory

### 🔧 **Getting Help**
- Use `!rolecontrol help` for complete command reference
- Check server permissions if features aren't working
- Ensure bot role is positioned correctly in role hierarchy

---

## 📈 Advanced Usage

### 🎨 **Customization**
- **Colors**: Use hex codes (#ff6b6b) for precise color matching
- **Templates**: Add custom templates by editing JSON files
- **Hierarchy**: Use position numbers to organize role order
- **Display**: Control role visibility with hoist and mentionable settings

### 📊 **Server Management**
- **Role Statistics**: Monitor role usage and member distribution
- **Bulk Operations**: Manage multiple roles efficiently
- **Permission Auditing**: Regular permission reviews for security
- **Template Standardization**: Consistent role setups across servers

---

*This documentation covers all features of the Role Control System. For technical implementation details, refer to the source code documentation.*
