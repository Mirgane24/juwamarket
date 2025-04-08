import React from "react";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Card, CardContent } from "@/components/ui/card";

export default function Home() {
  return (
    <main className="min-h-screen bg-white text-black p-6 md:p-12">
      <header className="flex justify-between items-center mb-12">
        <h1 className="text-3xl font-bold text-green-600">JuwaMarket</h1>
        <nav className="space-x-4">
          <Button variant="outline">Connexion</Button>
          <Button>S'inscrire</Button>
        </nav>
      </header>

      <section className="text-center max-w-3xl mx-auto mb-12">
        <h2 className="text-4xl font-bold mb-4">Vendez. Achetez. Payez en Bitcoin.</h2>
        <p className="text-lg text-gray-600 mb-6">
          Une plateforme e-commerce 100% Comorienne avec paiement via Lightning Network.
        </p>
        <div className="flex justify-center gap-2">
          <Input className="w-2/3" placeholder="Recherchez un produit ou un vendeur..." />
          <Button>Rechercher</Button>
        </div>
      </section>

      <section className="grid md:grid-cols-2 gap-6 max-w-5xl mx-auto">
        <Card>
          <CardContent className="p-6">
            <h3 className="text-xl font-semibold mb-2">Achetez depuis votre village</h3>
            <p className="text-gray-700">
              Même sans smartphone : achetez par code USSD et recevez vos produits rapidement.
            </p>
          </CardContent>
        </Card>
        <Card>
          <CardContent className="p-6">
            <h3 className="text-xl font-semibold mb-2">Vendez facilement</h3>
            <p className="text-gray-700">
              Mettez vos produits en ligne, fixez vos prix et recevez vos paiements en Bitcoin.
            </p>
          </CardContent>
        </Card>
      </section>

      <footer className="mt-20 text-center text-sm text-gray-500">
        © 2025 JuwaMarket - Une solution de commerce libre aux Comores.
      </footer>
    </main>
  );
}
