# GNSS Collision Detection System - Design Guidelines

## Design Approach
**Utility-Focused Design System**: This is a mission-critical safety application requiring clarity, efficiency, and immediate comprehension. Using **Material Design 3** principles with emphasis on data visualization and real-time status communication.

## Core Design Principles
- **Safety First**: Clear visual hierarchy for collision warnings
- **Real-time Clarity**: Instant comprehension of system status
- **Professional Reliability**: Enterprise-grade interface for fleet management
- **Responsive Monitoring**: Optimized for both desktop dashboards and mobile devices

## Color Palette

### Primary Colors
- **Primary**: 220 100% 45% (Deep blue for trust and reliability)
- **Surface**: 220 8% 97% (Light mode), 220 15% 8% (Dark mode)

### Status Colors
- **Success/Safe**: 142 75% 45% (Green for safe distances)
- **Warning**: 45 100% 50% (Amber for approaching threshold)
- **Danger/Collision**: 0 85% 55% (Red for collision alerts)
- **Neutral/Offline**: 220 10% 60% (Gray for inactive devices)

### Accent Colors
- **Info**: 200 100% 45% (Blue for informational states)
- **GPS Signal**: 275 85% 60% (Purple for GPS-related indicators)

## Typography
- **Primary Font**: Inter (Google Fonts)
- **Monospace**: JetBrains Mono (for coordinates and technical data)
- **Hierarchy**: Clear distinction between headings (24px), body (16px), and technical data (14px)

## Layout System
**Tailwind Spacing**: Primary units of 2, 4, 6, and 8 for consistent spacing
- Grid layouts for device cards and status panels
- Flexible dashboard layout accommodating map and device list
- Responsive breakpoints for mobile monitoring

## Component Library

### Core Components
- **Device Status Cards**: Real-time position and connection status
- **Collision Alert Banner**: Prominent warning system
- **Interactive Map**: Live tracking with device markers
- **Distance Monitor**: Real-time distance calculations display
- **Connection Status Indicator**: Network and GPS signal strength

### Navigation
- **Tab-based Dashboard**: Quick switching between views
- **Breadcrumb Navigation**: Clear location within system
- **Quick Actions Toolbar**: Emergency controls and settings

### Data Displays
- **Live Metrics Panel**: Distance, speed, GPS accuracy
- **Device List**: Sortable, filterable device management
- **Alert History**: Log of collision warnings
- **System Status**: Server health and connection quality

### Forms & Input
- **GPS Coordinate Input**: Manual entry forms
- **File Upload Interface**: GNSS logger file handling
- **Configuration Panel**: Threshold and alert settings

## Visual Treatments

### Map Integration
- **Dark base map** for better contrast with colored markers
- **Device markers**: Color-coded by status with clear labels
- **Proximity circles**: Visual representation of collision zones
- **Real-time trails**: Show recent movement paths

### Animations
- **Minimal and purposeful**: Pulsing alerts, smooth marker updates
- **Status transitions**: Gentle color changes for status updates
- **No distracting effects**: Focus on data clarity

### Responsive Behavior
- **Mobile-first dashboard**: Essential monitoring on phones
- **Desktop command center**: Full-featured control interface
- **Tablet-optimized**: Balanced view for field operations

## Critical Design Notes
- **High contrast ratios** for safety-critical information
- **Consistent dark mode** throughout application
- **Immediate visual feedback** for all user actions
- **Clear visual hierarchy** prioritizing collision warnings
- **Accessible color coding** with additional visual indicators beyond color alone