<script setup>
import { Button } from '@/components/ui/button'
import {FontAwesomeIcon} from "@fortawesome/vue-fontawesome";
import {
  Sheet,
  SheetContent,
  SheetTrigger,
} from '@/components/ui/sheet'
</script>

<template>
  <Sheet>
    <SheetTrigger>
      <Button class="lg:hidden md:hidden">
        <font-awesome-icon :icon="['fas', 'bars']" class="text-2xl" />
      </Button>
    </SheetTrigger>
    <SheetContent>

    </SheetContent>
  </Sheet>
</template>