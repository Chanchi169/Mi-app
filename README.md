<!DOCTYPE html>

<html class="light" lang="es"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>The Commander’s Ledger - Panel de Administración</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;700;800&amp;family=Inter:wght@400;500;600;700&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
      tailwind.config = {
        darkMode: "class",
        theme: {
          extend: {
            colors: {
              "on-tertiary": "#ffffff",
              "on-surface-variant": "#5b403d",
              "primary": "#91010e",
              "surface-container": "#eceef0",
              "surface-container-highest": "#e0e3e5",
              "on-tertiary-fixed-variant": "#00497e",
              "error": "#ba1a1a",
              "primary-container": "#b42323",
              "surface-container-low": "#f2f4f6",
              "inverse-on-surface": "#eff1f3",
              "tertiary-fixed": "#d2e4ff",
              "tertiary-container": "#0060a4",
              "secondary-fixed": "#d5e3fc",
              "on-secondary": "#ffffff",
              "on-surface": "#191c1e",
              "secondary": "#515f74",
              "tertiary-fixed-dim": "#a0caff",
              "error-container": "#ffdad6",
              "surface-dim": "#d8dadc",
              "surface": "#f7f9fb",
              "background": "#f7f9fb",
              "on-secondary-container": "#57657a",
              "on-tertiary-fixed": "#001c37",
              "on-primary-fixed-variant": "#92030f",
              "on-error": "#ffffff",
              "outline": "#8f706c",
              "on-secondary-fixed-variant": "#3a485b",
              "on-background": "#191c1e",
              "surface-variant": "#e0e3e5",
              "surface-tint": "#b52424",
              "on-error-container": "#93000a",
              "inverse-surface": "#2d3133",
              "on-primary-container": "#ffcac5",
              "outline-variant": "#e4beb9",
              "primary-fixed-dim": "#ffb4ac",
              "primary-fixed": "#ffdad6",
              "on-secondary-fixed": "#0d1c2e",
              "secondary-container": "#d5e3fc",
              "surface-container-lowest": "#ffffff",
              "surface-container-high": "#e6e8ea",
              "tertiary": "#00487d",
              "secondary-fixed-dim": "#b9c7df",
              "inverse-primary": "#ffb4ac",
              "surface-bright": "#f7f9fb",
              "on-primary-fixed": "#410003",
              "on-primary": "#ffffff",
              "on-tertiary-container": "#bed9ff"
            },
            fontFamily: {
              "headline": ["Manrope"],
              "body": ["Inter"],
              "label": ["Inter"]
            },
            borderRadius: {"DEFAULT": "0.125rem", "lg": "0.25rem", "xl": "0.5rem", "full": "0.75rem"},
          },
        },
      }
    </script>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
            vertical-align: middle;
        }
        .tonal-shift-only {
            background-color: rgba(247, 249, 251, 0.8);
        }
    </style>
<style>
    body {
      min-height: max(884px, 100dvh);
    }
  </style>
</head>
<body class="bg-surface font-body text-on-surface selection:bg-primary-container selection:text-on-primary-container">
<!-- TopAppBar -->
<header class="fixed top-0 w-full z-50 bg-slate-50/70 dark:bg-slate-900/70 backdrop-blur-md">
<div class="flex items-center justify-between px-6 h-16 w-full max-w-7xl mx-auto">
<div class="flex items-center gap-4">
<div class="w-10 h-10 rounded-full bg-surface-container flex items-center justify-center overflow-hidden border border-outline-variant/20">
<img alt="Fire Captain Profile" class="w-full h-full object-cover" data-alt="Portrait of a fire captain in uniform" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDQmKfYjMi1q3LQHPFHwYuCYryySvYOGDNhmxw_p0jxteOXH_0csUR4HNv3gmKabUsPAwdVA2H_-dLzo4i2JESfSNm1x_8wsZmQ8NAvK2J2VuK4FEUB6R2l9grgJI8GZQJod3rLFmwcyjsHJVrnUjvY4i-5eWB35p-pDzY6v5lFY0lnIxNxAOl7i_K1KF56IWbaYrGSGY6psCGCNzzwVaTzCoxnrZV47kgngoK5Oj91ynZtgMQ1fnkshHOX9wMO2xAwdbCe9ivWyQP4"/>
</div>
<h1 class="text-xl font-extrabold tracking-tighter text-red-900 dark:text-red-600 uppercase font-headline">The Commander’s Ledger</h1>
</div>
<button class="p-2 rounded-xl text-slate-500 hover:bg-slate-200/50 transition-colors active:scale-95 duration-150">
<span class="material-symbols-outlined" data-icon="notifications">notifications</span>
</button>
</div>
</header>
<main class="pt-24 pb-32 px-6 max-w-7xl mx-auto">
<!-- Header Section -->
<div class="mb-12">
<h2 class="text-4xl font-extrabold tracking-tight font-headline text-on-surface mb-2">Panel de Administración</h2>
<p class="text-secondary font-medium uppercase tracking-widest text-[10px]">Gestión Táctica de Flotas y Personal</p>
</div>
<!-- Bento Grid Layout -->
<div class="grid grid-cols-1 md:grid-cols-12 gap-6">
<!-- Quick Action: Generate Next Year -->
<section class="md:col-span-12 lg:col-span-4 bg-primary text-on-primary p-8 rounded-xl shadow-none relative overflow-hidden flex flex-col justify-between min-h-[320px]">
<div class="absolute top-0 right-0 w-32 h-32 bg-white/10 rounded-bl-full translate-x-8 -translate-y-8"></div>
<div class="relative z-10">
<div class="w-12 h-12 bg-white/20 rounded-lg flex items-center justify-center mb-6">
<span class="material-symbols-outlined text-3xl" data-icon="auto_mode">auto_mode</span>
</div>
<h3 class="text-2xl font-bold font-headline mb-3 leading-tight">Proyección Anual Automática</h3>
<p class="text-primary-container text-sm font-medium leading-relaxed opacity-90">
                        Calcula y genera el cuadrante completo para el próximo ciclo fiscal basándose en las rotaciones de equipo actuales y normativas de descanso.
                    </p>
</div>
<button class="relative z-10 mt-8 w-full py-4 bg-white text-primary font-bold rounded-lg hover:bg-surface-container-low transition-colors active:scale-95 flex items-center justify-center gap-3">
<span class="material-symbols-outlined" data-icon="calendar_add_on">calendar_add_on</span>
                    Generar Próximo Año
                </button>
</section>
<!-- Tool: Adjust Dates & Shifts -->
<section class="md:col-span-12 lg:col-span-8 bg-surface-container-low p-8 rounded-xl flex flex-col">
<div class="flex items-center justify-between mb-8">
<div>
<h3 class="text-xl font-bold font-headline text-on-surface">Ajuste de Calendario</h3>
<p class="text-on-surface-variant text-xs uppercase tracking-wider font-semibold mt-1">Sincronización de Turnos</p>
</div>
<div class="flex gap-2">
<button class="px-4 py-2 bg-surface-container-highest text-on-surface-variant text-sm font-bold rounded-lg border border-outline-variant/10">Mes Anterior</button>
<button class="px-4 py-2 bg-surface-container-highest text-on-surface-variant text-sm font-bold rounded-lg border border-outline-variant/10">Siguiente</button>
</div>
</div>
<div class="grid grid-cols-7 gap-2 mb-4 text-center">
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Lun</div>
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Mar</div>
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Mié</div>
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Jue</div>
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Vie</div>
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Sáb</div>
<div class="text-[10px] font-bold text-secondary tracking-widest uppercase">Dom</div>
</div>
<div class="grid grid-cols-7 gap-2 flex-grow">
<!-- Example Calendar Cells -->
<div class="aspect-square bg-surface-container-highest/40 rounded-lg flex flex-col p-2 border border-outline-variant/5">
<span class="text-xs font-bold text-on-surface-variant">28</span>
</div>
<div class="aspect-square bg-surface-container-highest/40 rounded-lg flex flex-col p-2 border border-outline-variant/5">
<span class="text-xs font-bold text-on-surface-variant">29</span>
</div>
<div class="aspect-square bg-surface-container-highest/40 rounded-lg flex flex-col p-2 border border-outline-variant/5">
<span class="text-xs font-bold text-on-surface-variant">30</span>
</div>
<div class="aspect-square bg-surface-container-lowest rounded-lg flex flex-col p-2 shadow-sm border border-outline-variant/10">
<span class="text-xs font-bold text-primary">1</span>
<div class="mt-auto h-1 w-full bg-tertiary rounded-full"></div>
</div>
<div class="aspect-square bg-primary-fixed rounded-lg flex flex-col p-2 border-b-2 border-primary">
<span class="text-xs font-extrabold text-on-primary-fixed-variant">2</span>
<div class="mt-auto flex gap-0.5">
<div class="h-1 w-2 bg-primary rounded-full"></div>
<div class="h-1 w-2 bg-secondary rounded-full"></div>
</div>
</div>
<div class="aspect-square bg-surface-container-lowest rounded-lg flex flex-col p-2 border border-outline-variant/10">
<span class="text-xs font-bold text-on-surface">3</span>
</div>
<div class="aspect-square bg-surface-container-lowest rounded-lg flex flex-col p-2 border border-outline-variant/10">
<span class="text-xs font-bold text-on-surface">4</span>
</div>
</div>
</section>
<!-- Personnel Management -->
<section class="md:col-span-12 lg:col-span-7 bg-surface-container-low p-8 rounded-xl">
<div class="flex items-center justify-between mb-8">
<h3 class="text-xl font-bold font-headline text-on-surface">Añadir Personal</h3>
<button class="flex items-center gap-2 text-primary font-bold text-sm hover:underline">
<span class="material-symbols-outlined text-lg" data-icon="person_add">person_add</span>
                        Alta Masiva
                    </button>
</div>
<div class="space-y-4">
<div class="flex flex-col gap-1.5">
<label class="text-[10px] uppercase font-bold tracking-widest text-secondary ml-1">Nombre del Efectivo</label>
<input class="w-full bg-surface-container-highest border-none rounded-sm px-4 py-3 text-on-surface placeholder:text-slate-400 focus:ring-1 focus:ring-primary/30" placeholder="Ej: Pedro García" type="text"/>
</div>
<div class="grid grid-cols-2 gap-4">
<div class="flex flex-col gap-1.5">
<label class="text-[10px] uppercase font-bold tracking-widest text-secondary ml-1">Rango / Rol</label>
<select class="w-full bg-surface-container-highest border-none rounded-sm px-4 py-3 text-on-surface focus:ring-1 focus:ring-primary/30">
<option>Oficial de Guardia</option>
<option>Bombero Especialista</option>
<option>Conductor de Autobomba</option>
</select>
</div>
<div class="flex flex-col gap-1.5">
<label class="text-[10px] uppercase font-bold tracking-widest text-secondary ml-1">Asignación de Grupo</label>
<select class="w-full bg-surface-container-highest border-none rounded-sm px-4 py-3 text-on-surface focus:ring-1 focus:ring-primary/30">
<option>Grupo Alfa</option>
<option>Grupo Bravo</option>
<option>Grupo Charlie</option>
</select>
</div>
</div>
<button class="w-full py-4 bg-primary text-on-primary font-bold rounded-md hover:bg-primary-container transition-all active:scale-[0.98] mt-4">
                        Confirmar Incorporación
                    </button>
</div>
</section>
<!-- Recent Changes / Audit Log -->
<section class="md:col-span-12 lg:col-span-5 bg-surface-container-lowest p-8 rounded-xl border border-outline-variant/10 shadow-[0_20px_40px_rgba(25,28,30,0.06)]">
<h3 class="text-xl font-bold font-headline text-on-surface mb-6">Actividad Reciente</h3>
<div class="space-y-6">
<div class="flex gap-4">
<div class="w-8 h-8 rounded-full bg-tertiary-fixed flex items-center justify-center shrink-0">
<span class="material-symbols-outlined text-on-tertiary-fixed-variant text-sm" data-icon="edit_calendar">edit_calendar</span>
</div>
<div>
<p class="text-sm font-bold text-on-surface">Cambio de Turno: B2 a B4</p>
<p class="text-xs text-secondary mt-1">Hace 12 minutos por Miller</p>
</div>
</div>
<div class="flex gap-4">
<div class="w-8 h-8 rounded-full bg-error-container flex items-center justify-center shrink-0">
<span class="material-symbols-outlined text-on-error-container text-sm" data-icon="person_remove">Baja Temporal: Bombero García</span>
</div>
<div>
<p class="text-sm font-bold text-on-surface">Baja Temporal: Bombero García</p>
<p class="text-xs text-secondary mt-1">Hace 2 horas • Motivo: Médico</p>
</div>
</div>
<div class="flex gap-4">
<div class="w-8 h-8 rounded-full bg-secondary-container flex items-center justify-center shrink-0">
<span class="material-symbols-outlined text-on-secondary-container text-sm" data-icon="groups">groups</span>
</div>
<div>
<p class="text-sm font-bold text-on-surface">Nuevo Grupo: Refuerzo Invierno</p>
<p class="text-xs text-secondary mt-1">Ayer a las 18:30</p>
</div>
</div>
</div>
</section>
</div>
</main>
<!-- BottomNavBar -->
<nav class="fixed bottom-0 left-0 w-full flex justify-around items-center px-4 pb-6 pt-3 bg-white/80 dark:bg-slate-900/80 backdrop-blur-lg z-50 shadow-[0_-10px_30px_rgba(25,28,30,0.04)] border-t border-slate-200/30 dark:border-slate-800/30">
<a class="flex flex-col items-center justify-center text-slate-500 dark:text-slate-500 px-4 py-1.5 hover:text-red-700 transition-colors active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined mb-1" data-icon="dashboard">dashboard</span>
<span class="font-['Inter'] font-semibold text-[10px] tracking-wider uppercase">Dashboard</span>
</a>
<a class="flex flex-col items-center justify-center text-slate-500 dark:text-slate-500 px-4 py-1.5 hover:text-red-700 transition-colors active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined mb-1" data-icon="event_repeat">event_repeat</span>
<span class="font-['Inter'] font-semibold text-[10px] tracking-wider uppercase">Rotations</span>
</a>
<a class="flex flex-col items-center justify-center text-slate-500 dark:text-slate-500 px-4 py-1.5 hover:text-red-700 transition-colors active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined mb-1" data-icon="groups">groups</span>
<span class="font-['Inter'] font-semibold text-[10px] tracking-wider uppercase">Profiles</span>
</a>
<a class="flex flex-col items-center justify-center bg-red-50 dark:bg-red-950/30 text-red-900 dark:text-red-400 rounded-xl px-4 py-1.5 transition-all active:scale-90 duration-200" href="#">
<span class="material-symbols-outlined mb-1" data-icon="admin_panel_settings" style="font-variation-settings: 'FILL' 1;">admin_panel_settings</span>
<span class="font-['Inter'] font-semibold text-[10px] tracking-wider uppercase">Admin</span>
</a>
</nav>
</body></html>
